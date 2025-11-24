# 🎮 Pixel Defense: Hardcore Edition

> A fast-paced tower defense game built with vanilla JavaScript and HTML5 Canvas

![Game Status](https://img.shields.io/badge/status-active-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Version](https://img.shields.io/badge/version-1.0.0-orange)

## ✨ Features

### 🏰 Tower Types (4 Variants)

| Tower | Cost | Range | Damage | Special Ability |
|-------|------|-------|--------|-----------------|
| **Turret** | 50$ | 120px | 20 | Dual shot (Lv2) |
| **Sniper** | 120$ | 300px | 100 | Instant kill chance (Lv2) |
| **Blaster** | 200$ | 90px | 10 | Slow effect (Lv2) |
| **Artillery** | 250$ | 275px | 80 | Napalm zones (Lv2) |

### 👾 Enemy Types (10 Variants)

```
🟢 Basic        - Standard enemy
🟣 Swarm        - Fast & weak
🟡 Fast         - High speed
🔵 Tank         - Tanky & slow
🟢 Armored      - Extra armor
⚫ Drone        - Flies (sniper only)
🟢 Buffer       - Shields allies
🔴 Exploder     - Destroys towers
👑 Boss         - Wave 10, 20, 30...
☠️  Super Boss  - Wave 25 (ultimate)
```

### 🎯 Game Mechanics

- **Wave System**: 25 progressively harder waves
- **Tower Upgrades**: Upgrade towers to level 2 for special abilities
- **Sell System**: Recover 50% of invested money
- **Sound Effects**: Web Audio API for dynamic audio
- **Particle Effects**: Visual feedback for all actions
- **Economy**: Earn money from defeated enemies
- **Map Size**: Large 1600×1000px grid with complex pathfinding

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No additional dependencies required!

### Quick Start

#### Option 1: Direct Browser Open
```bash
# Navigate to the project directory and double-click index.html
```

#### Option 2: Local Server
```bash
# Python 3
python3 -m http.server 8000

# Then visit: http://localhost:8000
```

#### Option 3: Node.js (http-server)
```bash
npm install -g http-server
http-server
```

## 🎮 How to Play

### Controls
- **Select Tower**: Click on tower buttons on the left panel
- **Place Tower**: Click on the map to build
- **Select Tower**: Click on existing tower to select it
- **Upgrade Tower**: Click "УЛУЧШИТЬ" (Upgrade) button
- **Sell Tower**: Click "ПРОДАТЬ" (Sell) button
- **Start Wave**: Click "▶ СТАРТ ВОЛНЫ" button

### Strategy Tips
- 💰 Start with **Turrets** to get early money
- 🎯 Use **Snipers** for high damage output
- ❄️ Use **Blasters** for crowd control (slowing)
- 💣 Use **Artillery** for area damage and napalm zones
- 🛡️ Balance your tower placement for coverage
- 📈 Upgrade towers strategically for special abilities

## 🎨 Game UI

```
┌─────────────────────────────────────────────────┐
│  ⚡ Pixel Defense: Hardcore Edition              │
├─────────────────────────────────────────────────┤
│  ❤️  Lives: 20    💰 Money: 300    🌊 Wave: 0  │
├─────────────────────────────────────────────────┤
│                    CANVAS AREA                   │
│                   (1600×1000px)                  │
│                                                  │
├─────────────────────────────────────────────────┤
│  [Turret] [Sniper] [Blaster] [Artillery] [START]│
└─────────────────────────────────────────────────┘
```

## 🛠️ Technical Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript (ES6+)
- **Graphics**: HTML5 Canvas 2D
- **Audio**: Web Audio API
- **Architecture**: Object-Oriented (Classes)

## 📁 Project Structure

```
Js Game1/
├── index.html          # Main game file (all-in-one)
├── Game.js            # Legacy version (deprecated)
└── README.md          # This file
```

## 🎓 Class Architecture

### Core Classes

```javascript
// Main game controller
class Game { }

// Enemy logic
class Enemy { }

// Tower logic
class Tower { }

// Projectile system
class Projectile { }
class ArtilleryProjectile { }

// Visual effects
class Particle { }
class NapalmZone { }

// Audio manager
class SoundManager { }
```

## 📊 Game Progression

### Wave Structure
```
Waves 1-9    → Basic enemies with variations
Wave 10      → First Boss + 10 fast enemies
Waves 11-19  → Harder enemy types
Wave 20      → Boss wave
Waves 21-24  → Maximum difficulty
Wave 25      → Super Boss (ultimate challenge)
```

### Difficulty Scaling
- Enemy HP increases: `baseHP × (1 + wave × 0.3)`
- Enemy spawn rate: 25 frames between spawns
- Boss waves: 120 frames between boss spawns

## 🎵 Audio Effects

The game includes procedural audio generation for:
- 🔫 Tower shots (Sniper, Turret, Blaster, Artillery)
- 💥 Explosions
- ⚡ Critical hits
- 💀 Enemy deaths
- 🔨 Tower building
- 📢 UI interactions

## 🐛 Known Limitations

- Single player only
- No pause functionality
- No save/load system
- No difficulty settings
- Audio may not work in some browsers without HTTPS

## 🔄 Future Enhancements

- [ ] Pause functionality
- [ ] Settings menu (sound toggle, difficulty)
- [ ] Leaderboard system
- [ ] More tower types
- [ ] Different map layouts
- [ ] Mobile support
- [ ] Multiplayer mode
- [ ] Custom game modes

## 📈 Performance

- **FPS**: 60 FPS (requestAnimationFrame)
- **Canvas Size**: 1600×1000 (optimized rendering)
- **Particle System**: Up to 1000 particles
- **Enemy Limit**: 200+ enemies per wave

## 🤝 Contributing

Contributions welcome! Feel free to:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

MIT License - feel free to use this project for personal or commercial purposes.

## 👨‍💻 Author

**AlexZ671** - Tower Defense Game Developer

## 🔗 Links

- 🎮 [Play Online](http://localhost:8000)
- 📚 [GitHub Repository](https://github.com/AlexZ671/GameTowar)
- 📧 Contact: alexz671@example.com

## 🏆 Credits

- Game design and implementation: AlexZ671
- Built with vanilla JavaScript and HTML5 Canvas
- No external libraries required

---

<div align="center">

**⭐ If you enjoy this game, please consider giving it a star!**

**Made with ❤️ by AlexZ671**

</div>
