# Ez GG Datapack Bots

A Minecraft datapack that lets you spawn and control bots that fight you.

---

## 📥 Download V1

1. [Download V1](https://github.com/CreeperGamingDT/Ez-gg-inv/raw/main/ez-gg-botsv1.zip)  
2. Open your Minecraft worlds folder  
3. Open the `datapacks` folder  
4. Drag the downloaded `.zip` file into `datapacks`  
5. Run `/reload` in-game  

---
## 📥 Download V2 (Experimental)

1. [Download V2 (Experimental)](https://github.com/CreeperGamingDT/Ez-gg-inv/raw/main/ez-gg-botsv2.zip)  
2. Open your Minecraft worlds folder  
3. Open the `datapacks` folder  
4. Drag the downloaded `.zip` file into `datapacks`  
5. Run `/reload` in-game  
### This version may be outdated and will not be documented.
---
# V1 Documentation

## 🚀 Quick Start

Recommended setup order:

1. `/function players:setup`
2. `/function players:spawn`
3. `/function players:setuplevel`
4. Optional: add targeting tag
5. Start fighting bots

---

## 🤖 Features

- Spawn bots that fight players
- Full bot control system (kill, stop, disconnect, etc.)
- Targeting system (priority / ignore player)
- Bot setup & restocking system
- Utility tools for testing and debugging
- Designed for survival PvP testing

---

## ⚙️ Commands

# 🧪 Setup

### Initialize System
```mcfunction
/function players:setup
````

Sets up scoreboards, teams, and bot systems.

---

### Spawn Bots

```mcfunction
/function players:spawn#
```

Spawns 25 bots into the world.
Replace ``#`` with a number 1-5

---

### Setup Bot Roles

```mcfunction
/function players:setuplevel
```

Assigns bot tags and behavior roles.

---

## 🎯 Targeting System

### Disable Bot Targeting

```mcfunction
/tag @s add team1notattack
```

Bots will stop targeting you. (Will target other players)

---

### Enable Priority Targeting

```mcfunction
/tag @s add team1attack
```

Makes you the highest priority target. (Will not target other players without tag)

---

## ⚔️ Bot Control

### Stop Bots

```mcfunction
/function players:stop
```

Stops all bot actions. (If not actively targeting)

---

### Kill All Bots

```mcfunction
/function players:kill
```

---

### Kill A Random Bot

```mcfunction
/function players:killrandom
```

---

### Damage All Bots

```mcfunction
/function players:killdrop
```

Applies heavy damage to all bots (kills them).

---

### Damage A Random Bot

```mcfunction
/function players:killdroprandom
```
Applies heavy damage to a random bot (kills them).
---

### Disconnect All Bots

```mcfunction
/function players:disconnect
```

Removes all bots from the world. (Alternative when running the datapack on a server)

---

## 🔧 Bot Fixes & Utilities

### Fix Golden Apple Behavior

```mcfunction
/function players:fixgap
```

Forces bots to use golden apples correctly. (Useful when bots are holding a golden apple and not eating)

---

### Teleport Far Bots Back

```mcfunction
/function players:tpfar
```

Teleports distant bots back near the player. (50 blocks away)

---

### Force Bots to Look At You

```mcfunction
/function players:look
```

Makes all bots face the player.

---

## 📝 Notes

* Designed for Minecraft Java Edition 1.21+
* Bots require setup before spawning properly
* Some features may be experimental depending on version
