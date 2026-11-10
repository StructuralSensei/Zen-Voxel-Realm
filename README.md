# 🌲 Zen Voxel Realms

**A free, cozy, open-world voxel sandbox that runs in your browser from a single HTML file.**
Wander, build a cabin, fish in the river, hunt for dinner, catch creatures with Poké Balls, then lie down and watch the sun go down. No install, no accounts, no ads.

<p align="center">
  <!-- 🎬 HERO GIF: 10–15s loop of walking through the world at golden hour -->
  <img src="preview.gif" alt="Zen Voxel Realms gameplay" width="800">
</p>

<p align="center">
  <a href="#-play-now"><b>Play now</b></a> ·
  <a href="#-features">Features</a> ·
  <a href="#-controls">Controls</a> ·
  <a href="#-run-it-locally">Run locally</a> ·
  <a href="#-roadmap">Roadmap</a>
</p>

---

## ▶ Play now

Download `zen-voxel-realms.html` and double-click it. That's the whole setup.

---

## ✨ Features

### 🧘 Relax
- Slow day and night cycle with fireflies after dark
- Rain you can toggle, with a quieter, moodier sky
- Campfires that flicker and crackle
- Rest mode, a photo mode that hides the HUD, and fully procedural ambient sound (wind, birdsong, water, footsteps), with no audio files
- Swim, fly, walk, or just sit by the river

<p align="center">
  <!-- 📸 SCREENSHOT: night scene with campfire + fireflies -->
  <img src="docs/media/night-campfire.png" alt="Campfire at night with fireflies" width="390">
  <!-- 📸 SCREENSHOT: rain over the river and bridges -->
  <img src="docs/media/rain-river.png" alt="Rain over the river" width="390">
</p>

### 🧱 Build
- Place and remove blocks smoothly: hold the mouse button to keep building
- A ghost outline shows exactly where a block will land
- Eight materials, including **doors** that open, **beds** you can sleep in, and **windows**
- A starter cabin to explore (or tear down)
- Real collisions: you walk around things, step over low obstacles, and jump to climb

<p align="center">
  <!-- 🎬 GIF: placing blocks to build a small house, opening the door -->
  <img src="docs/media/building.gif" alt="Building a house" width="600">
</p>

### 🎣 Survive
- Health, hunger and air bars
- Real swimming, and **you can drown** if you stay under for more than 30 seconds
- Fall damage, starvation, and sleeping in a bed to heal and skip the night
- Pick **apples and oranges** from trees (they regrow)
- **Fish** in the river
- **Hunt** pigs, chickens, deer and birds with a **sword or a bow**. Arrows really fly, arc, and can be picked back up
- Cook meat at a campfire for a bigger meal
- A two-sided **inventory**: Poké Balls and partners on one side, food and supplies on the other

<p align="center">
  <!-- 📸 SCREENSHOT: inventory panel -->
  <img src="docs/media/inventory.png" alt="Inventory screen" width="390">
  <!-- 🎬 GIF: shooting a bird with the bow -->
  <img src="docs/media/bow.gif" alt="Shooting a bird with the bow" width="390">
</p>

### 🔴 Catch & battle
- Wild creatures wander the map in three elements: **Fire, Water, Grass**
- Walk into one to start a turn-based standoff
- Pick **Fight**, throw a **Poké Ball**, or **Run**
- Every action is decided by a **D20 roll**: misses on low rolls, crits on a 20
- Type advantages: Fire > Grass > Water > Fire
- Caught creatures follow you, level up, and fight for you. Rest to heal them

<p align="center">
  <!-- 🎬 GIF: full battle sequence ending in a successful catch -->
  <img src="docs/media/battle-catch.gif" alt="Battle and catch sequence" width="600">
</p>

### 🌍 A living world
- Rivers with bridges, forests, rocks, flowers, wandering animals, circling birds, and fish that leap in the water
- Villagers with a little advice
- Poké Ball pickups scattered around the map
- First-person and third-person views

---

## 🎮 Controls

| Action | Key |
|---|---|
| Move | `W` `A` `S` `D` |
| Look | Mouse (click the game to capture it) |
| Jump / swim up | `Space` |
| Sprint / dive underwater | `Shift` |
| Fly on/off | `F` |
| Rest (heals partners) | `R` |
| First / third person | `V` |
| Use: open door, sleep, pick fruit, eat | `E` |
| Inventory | `I` |
| Cycle tool (build → sword → bow) | `Z` |
| Select block | `1`–`8` |
| Place / attack / shoot | Left click |
| Remove block | Right click |
| Light a campfire | `C` |
| Fish | `G` (press again when you see the bite!) |
| Toggle rain | `T` |
| Photo mode | `P` |
| Zoom camera | Mouse wheel |
| Menu & settings | `Esc` |

<p align="center">
  <!-- 📸 SCREENSHOT: pause menu with settings -->
  <img src="docs/media/menu.png" alt="Menu and settings" width="500">
</p>

---

## 🛠 Run it locally

No build tools needed.

```bash
git clone https://github.com/YOUR-USERNAME/zen-voxel-realms.git
cd zen-voxel-realms
# open the file in any modern browser:
open zen-voxel-realms.html        # macOS
xdg-open zen-voxel-realms.html    # Linux
start zen-voxel-realms.html       # Windows
```

Want to host it? Enable **GitHub Pages** (Settings → Pages → deploy from `main`) and rename the file to `index.html`.

**Requirements:** a desktop browser with WebGL and mouse pointer-lock support (Chrome, Edge, Firefox, Safari). An internet connection is needed on first load to fetch Three.js from a CDN.

---

## 🧩 How it's built

- **One file.** HTML, CSS and JavaScript in a single document
- **[Three.js](https://threejs.org/)** (r160 from cdnjs) for rendering
- **Zero image or model files.** Textures are drawn at runtime on `<canvas>`, characters and animals are built from boxes
- **Zero audio files.** Sound is synthesized with the Web Audio API
- Turn-based battles run as an HTML/CSS overlay on top of the 3D scene

---

## 🗺 Roadmap

- [ ] Save and load your world
- [ ] Crafting (arrows, tools, cooked meals)
- [ ] More creature types, moves and evolutions
- [ ] Creature collection screen
- [ ] Enemies and a danger-free "zen mode" toggle
- [ ] Gamepad and mobile touch controls
- [ ] Seeded random worlds and bigger maps
- [ ] Optional multiplayer

Have an idea? [Open an issue](../../issues).

---

## 🤝 Contributing

Pull requests are welcome. Because the game is a single file, keep changes focused and test in at least one Chromium and one non-Chromium browser. Please include a screenshot or GIF for visual changes.

---

## 📜 License

Released under the [MIT License](LICENSE). Free to play, remix and share.

*This is a fan-inspired project and is not affiliated with or endorsed by Nintendo, The Pokémon Company, or Wizards of the Coast. "Poké Ball" is used descriptively for a creature-catching mechanic. Swap the name if you plan to distribute commercially.*

---

<p align="center">Made for slow evenings. 🌙 If you enjoy it, ⭐ the repo!</p>
