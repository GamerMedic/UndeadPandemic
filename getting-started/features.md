# 🧰 Features

1. <mark style="color:orange;">**Zombie Spawning**</mark>**:**
   * Zombies can spawn based on a configurable rate (`zombies.spawn-rate`).
   * **Custom Zombies:** You can customize the zombies' appearance and attributes using the `ZombieType` enum. Custom zombies are spawned based on a configurable chance.
   * **Vanilla Zombies:** Regular vanilla zombies can also spawn based on configuration.
   * Zombies spawn faster during specific events, like full moons.
   * **Blood Moon Event:** During a full moon, there is a chance for zombies to spawn more frequently, triggering faster zombie spawning (custom spawn rate). This event is configurable, including the chance (`zombies.events.blood-moon.horde-chance`).
2. <mark style="color:blue;">**Thirst System**</mark>**:**
   * Players have a **thirst level** that depletes over time.
   * The rate of thirst depletion is configurable (`thirst.dehydration_rate`) and varies depending on whether the player is premium or not.
   * Premium players lose thirst at a **slower rate** (`thirst.dehydration_amount`).
   * Thirst drops lead to players experiencing **debuffs** like Confusion and Weakness if their thirst falls below certain thresholds.
   * The thirst system updates periodically, and players receive **warning** messages when their thirst is dangerously low.
   * Thirst is tracked and updated using a **boss bar** for each player.
   * Thirst changes are persisted in memory and saved to ensure consistency across sessions.
3. <mark style="color:purple;">**Moon Phase Monitoring**</mark>**:**
   * The plugin checks the current **moon phase** of the world and adjusts gameplay accordingly.
   * During a **full moon**, zombies spawn at a **higher rate** (accelerated spawn rate).
   * A random chance determines whether the full moon event actually triggers the faster spawn rate, adding an element of unpredictability to the gameplay.
4. <mark style="color:yellow;">**Premium Features**</mark>**:**
   * **Faster Thirst Depletion:** Premium players experience a slower rate of thirst loss (`thirst.premium_dehydration_amount`).
   * **Custom Zombie Spawning:** Premium players can experience unique custom zombies, possibly linked to different world events or conditions, like the moon phase.
   * **Dehydration Buffers:** Premium users may get more lenient mechanics for dealing with thirst, including custom debuffs and longer time to reach critical thirst levels.
   * **Exclusive Events:** Certain events, such as faster zombie spawning during the blood moon, might be more rewarding or frequent for premium players.
5. <mark style="color:purple;">**Plugin Configuration**</mark>**:**
   * The plugin heavily relies on the `config.yml` file for configuring the spawn rate of zombies, thirst mechanics, moon phase checks, and events.
   * Key configurable options include:
     * **Zombie spawn rates and chances.**
     * **Thirst max, buffer, and warning thresholds.**
     * **Moon phase-related events** (accelerated spawn rates, event chances).
6. <mark style="color:green;">**Player Interactions and Feedback**</mark>**:**
   * The plugin provides in-game **feedback** via messages when players reach low thirst levels, with **warnings** and **buffer alerts**.
   * The plugin also **customizes player experiences** using **potion effects** (like Confusion and Weakness) when their thirst is dangerously low.
   * Premium users may receive different levels of feedback or notifications tailored to their gameplay experience.

#### <mark style="color:yellow;">Premium</mark> vs. <mark style="color:orange;">Non-Premium</mark> Features:

* **Premium Players:**
  * Slower thirst depletion rate.
  * Enhanced zombie spawning and more frequent events (e.g., blood moons).
  * Custom zombies with unique types and attributes.
  * Special debuffs or extended mechanics related to thirst.
* **Non-Premium Players:**
  * Standard thirst depletion rate.
  * Vanilla and occasional custom zombies spawning.
  * Standard moon phase mechanics and zombie spawning
