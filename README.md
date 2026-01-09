# The Mining Dead - Game Design Document (GDD) [Version 2.0]

**Title**: The Mining Dead  
**Genre**: Zombie Apocalypse Survival / Colony Building Hybrid  
**Platform**: Hytale (Modpack/Mod + Dedicated Server)  
**Target Audience**: Hardcore survival fans, Walking Dead enthusiasts, Minecraft modders transitioning to Hytale  
**Core Loop**: Scavenge → Fortify → Survive → Rebuild → Repeat  
**Tagline**: *How long will you survive when the dead keep digging deeper?*  
**Discord**: https://discord.gg/gCRv62araB (**Actively recruiting: Developers, Model Designers, Builders** - solo dev needs help!)  
**Status**: Pre-Launch (Tied to Hytale Early Access on January 13, 2026)  
**Note**: All features depend on Hytale's modding APIs. Subject to change.

---

## 🎬 Story & Setting

> The world has fallen to decay. Civilization crumbled years ago, leaving behind shattered cities, broken roads, and the endless moans of the undead. What remains of humanity hides among the ruins—desperate, starving, and slowly losing hope.  
> 
> You are one of the survivors, traveling through once-bustling **mining towns** now crawling with the infected. Scavenge for supplies, craft weapons from scraps, and uncover what's left of the old world. Every step into the darkness brings new risks and new choices.  
> 
> **Inspired by The Walking Dead × 28 Days/Weeks/Years Later**

---

## 🎯 Core Gameplay Pillars

| Pillar              | Description                                      |
|---------------------|--------------------------------------------------|
| **🧭 Tense Resource Scavenging** | Multi-level high-risk structures & cities—deeper/dangerous areas hold better loot. Noise-based zombie attraction (block breaking, footsteps, gunfire, **mining generates noise attracting nearby walkers**). Dynamic loot tiers: rusty tools → rare industrial gear → legendary pre-outbreak tech. |
| **🏘️ Colony Building & Defense** | **Towny/Minecolonies-style system** for Hytale: Build towns, upgrade buildings, manage NPC citizens who help fight/defend. Fortify mining towns with barricades, flood traps. Town claims with taxes, roles, and betrayal mechanics. Massive herd events test fortifications (300+ walkers). |
| **🦠 Infection & Progression** | Bite wounds → fever → amputation → death (or turn). **Idea**: Players turn into controllable zombies attacking friends, or respawn as fresh survivors with memory loss? Skill trees: Miner (better ore yields), Survivor (stealth/crafting), Warlord (leadership/combat). Day/night/weather cycles amplify difficulty. |

---

## 👾 Zombie/Walker Mobs & AI

- 🐌 **WALKERS** - Slow shamblers, attracted to noise/light, **break blocks over time**.
- 🏃 **RUNNERS/Fresh Infected** - Fast sprinters, climb walls, **break blocks faster**.
- 💥 **BLOATED/Gore Walkers** - Explosive on death, spread infection.
- 🛡️ **ARMORED/Elite Walkers** - Wear scrap armor, resist melee, **highest block damage**.
- 🌊 **HERDS** - Mass spawns triggered randomly, scaled by POI zones: Zone 1=1-3 zombies, Zone 2=8-12, Zone 3=15-25+.
- **Zombie Awareness**: Noise/radiation/scent detection systems.

**Mining Integration**: Unsecured shafts risk ceiling collapses—players must reinforce tunnels with beams/supports. Mining noise attracts swarms.

---

## 🛠️ Key Systems & Features

### 🔨 Block Upgrade System
- **WOOD** barricades (weakest, ~2min break time)  
- **STONE** (~5min)  
- **CONCRETE** (~10min)  
- **IRON** (~20min)  
- **STEEL** (strongest, ~45min+)

### 🚗 Vehicle Progression
- 🚲 Bicycle  
- 🛵 Moped  
- 🏍️ Motorcycle  
- 🚙 Jeep  
- 🚁 Helicopter/Planes

### 🏘️ Towny + NPCs & Factions
- Build colonies, upgrade buildings.
- NPC citizens auto-defend/manage buildings.
- Taxes, roles, faction betrayals.
- Reputation with rival colonies.
- POI danger zones (Zone 1→Zone 5).
- Trader caravans & bandit raids.
- **Friendly/Aggressive Colonies**: Trading/raiding with **reputation system** (trade supplies = +rep, betrayals = -rep, unlocks interactions).

### 🦠 Brutal Survival Mechanics
- Full system: Thirst, Hunger, Temperature (realistic needs).
- Infection: Bite → Fever → Amputation → ? (Details TBD: Cure chances, turning mechanics).
- Day/Night Cycle: Walkers stronger at night, hordes at dusk.
- Weather Events: Rain hides noise, fog reduces vision, storms spawn specials.
- **Performance Note**: Monitor walker cap per chunk once Hytale launches.

### 📦 Items & Weapons
- **Melee**: Baseball bats, machetes, crowbars, pipe bombs.
- **Ranged**: Crossbows, scrap guns, molotovs, silenced pistols.
- **Medical**: Bandages, antibiotics, painkillers, blood bags.
- **Utility**: Walker's guts (camouflage), radio (locate traders), backpack expansions.
- **Blocks & Structures**: Chain-link fences, razor wire, sandbag walls, traps (spike pits, tripwires, noise makers), generators (power lights, turrets, crafting stations).

### 👥 NPCs & Factions
- Survivor NPCs (tradeable, joinable groups with quests).
- Bandit Raiders (hostile human PvE, steal loot).
- Trader Caravans (mobile shops with rare items).
- Safe Zone Leaders (protect towns for tribute).

---

## 📋 Launch Features

- ✅ Core Walkers + block-breaking AI.
- ✅ Basic barricades (WOOD→STONE).
- ✅ Day 1 Server live at launch.
- ✅ Noise system (mining alerts zombies).
- ✅ Survival basics (hunger/thirst).

**Week 1-4 Post-Launch:** Towny • Vehicles • Infection.  
**Beta:** Herds • Factions • POI Zones.

---

## 🎨 Art Direction

- 🔴 Gritty industrial decay.
- ⚒️ Rusted mineshafts + ore veins.  
- 🌫️ Foggy ruined cities + barricade chaos.
- 🔊 Distant moans + echoing pickaxes.

---

## 🚀 Development Roadmap

- 📅 **LAUNCH DAY**: Core Survival (Tied to Hytale Early Access, Jan 13, 2026).
- 📈 **Week 1-4**: Towny + Vehicles.  
- 🧪 **Beta**: Factions + POI Zones.
- 🎉 **1.0**: Herds + Mining Dangers.
- 🌟 **Future**: Underground dangers, TWD-themed custom server, world states & difficulty scaling (e.g., POI zones with escalating threats).

**No ETA Beyond Launch** - Depends on Hytale modding APIs and team growth.

---

## ⚠️ Development Notes

- **Balance Considerations**: Tune break times, horde sizes, and resource scarcity based on playtesting. Ensure new players aren't overwhelmed by early sieges.
- **Technical Dependencies**: Relies on Hytale's modding tools for AI, block interactions, and NPCs. Monitor for performance with large herds.
- **Monetization Ideas**: Passion project—potential future revenue via donations, premium servers, or player growth (e.g., Patreon for early access).
- **Active Development**: All features PLANNED but NOT FINAL. Rapid updates post-launch.

---

## 👥 Join the Development Team!

**Solo developer needs help!** 💪

| Role          | Skills                          |
|---------------|---------------------------------|
| 💻 Developer  | Hytale scripting, mob AI       |
| 🎨 Modeler    | Zombies, weapons, vehicles     |
| 🏗️ Builder   | Towns, POIs, mineshafts        |

**Compensation:** Passion project → Future revenue share (player growth, donations, premium servers).  
**Join Discord:** https://discord.gg/gCRv62araB

---

*The dead keep digging deeper. Will your colony survive?* 🧟‍♂️⚒️