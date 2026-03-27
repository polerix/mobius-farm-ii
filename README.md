# 🌊 MÖBIUS MUSHROOM FARM 🌊

💧 An ASCII-based farming & tower-defense hybrid game running entirely in the browser, flowing with the tide. 🫧

## 🐚 Overview

Manage two surfaces connected by a Möbius edge. Cultivate mushrooms, defend against enemies (centipedes and pyramids), and optimize your farm stability. The game blends resource management, real-time strategy, and ecological simulation across the waves. 🌊

## 💧 Game Mechanics

### 🐚 Core Gameplay
- **Two Surfaces**: Top and bottom surfaces separated by a Möbius edge (wrapping logic flips surfaces and mirrors Y coordinates) 🫧
- **Player**: Positioned on the edge line, controls a train with a turret
- **Resources**: Energy, Shield, Pods (charged power cells) 🐚

### 🌊 Mushroom Life Cycle
1. **Spore** (`.`) → **Seed** (`,`) → **Mushroom** (`m/M/Ø` - stages 1-3) → **Burst** (`*` flash) 💧
2. **Growth**: Natural aging over time, accelerated by player shots, enemy interactions 🫧
3. **Burst**: Automatic at max stage or age; creates AoE damage to enemies and spreads new spores 🐚

### 🐚 Enemies
- **Centipede** (`@` head, `*` segments): Long, tracking predator that damages mushrooms 🌊
- **Pyramid** (`Δ`): Harasser that fires torpedoes toward the edge 💧

### 🫧 Player Actions
- **Move** (`← →` / `A D`): Slide along the edge 🐚
- **Aim** (`W/S`): Switch which surface you shoot into (up or down) 🌊
- **Fire** (`Space`): Shoot mushrooms to accelerate growth, or enemies to destroy them 💧
- **Defrag Pulse** (`Enter`): Move spores/seeds toward mushroom clusters (costs energy) 🫧
- **Pause** (`P`): Pause the game 🐚
- **Restart** (`R`): Reset 🌊

### 🐚 Economy
- **Stability Meter**: Tracks farm density (optimal around 55%) 💧
- **Energy**: Recharges slowly; fuels firing, defrag-tool, shield regen 🫧
- **Shield**: Absorbs damage; regenerates if you have surplus energy 🐚
- **Pods**: Charge when energy > 45; auto-launch at 100% for score bonus 🌊

## 🌊 Technical

- **Single-File HTML5**: Entire game in one `.html` file 💧
- **No Dependencies**: Pure JavaScript, no frameworks 🫧
- **Rendering**: ASCII characters in a `<pre>` element with monospace font 🐚
- **Audio**: Simple square-wave beeps (Web Audio API) 🌊
- **Timing**: 30 FPS game loop with proper delta-time accumulation 💧

## 🐚 How to Play

1. Open `index.html` in a modern web browser 🫧
2. Allow audio permissions when prompted (for game sounds) 🐚
3. Start with a seeded farm; manage growth and defense 🌊
4. Keep farm stability between 40–60% for best results 💧
5. Rack up score by bursting mushrooms and destroying enemies 🫧

## 💧 Configuration

Edit these constants in the `<script>` section to tweak gameplay: 🐚
- `W`, `H`: Grid dimensions 🌊
- `ENERGY_MAX`, `SHIELD_MAX`: Resource caps 💧
- `FIRE_COST`, `DEFRAG_COST`: Action costs 🫧
- `SPORE_TO_SEED_TICKS`, `SEED_TO_MUSH_TICKS`: Growth timings 🐚
- `CENTI_LEN_START`, `PYRAMID_SPAWN_TICKS`: Enemy parameters 🌊
- `MOBIUS_MIRROR_Y_ON_WRAP`: Enable/disable Y mirroring on Möbius wrap 💧

## 🐚 Tips

- **Balance**: Too sparse = starving; too dense = chaos. Aim for ~55% density. 🫧
- **Defense**: Focus shots on enemies before they reach your farm. 🐚
- **Growth**: Nurturing mushrooms (shooting them early) is rewarded with resource gains. 🌊
- **Defrag**: Use the defrag-tool pulse strategically when you have energy surplus to reorganize your farm. 💧
- **Combo**: Consecutive enemy kills boost score exponentially. 🫧

## 🌊 License

Created as a game design prototype. Feel free to fork, mod, and share! 🐚

---
*Be like water, my friend. It can flow or it can crash.* 🌊
