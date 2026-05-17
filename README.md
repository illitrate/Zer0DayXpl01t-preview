<p align="center">
  <img src="AppIcon.png" width="120" height="120" alt="Zer0Day Xpl01t App Icon"/>
<br/>
  <img src="SplashScreen Medium.png" width="640" height="427" alt="Zer0Day Xpl01t App Icon"/>
</p>

<h1 align="center">Zer0Day Xpl01t</h1>

<p align="center">
  <em>A cyberpunk hacking game for iOS built with SwiftUI</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-iOS-blue" alt="Platform: iOS"/>
  <img src="https://img.shields.io/badge/swift-SwiftUI-orange" alt="SwiftUI"/>
  <img src="https://img.shields.io/badge/status-In%20Development-green" alt="Status: In Development"/>
</p>

---

Step into a neon-soaked dystopia where megacorporations control everything and the only power left belongs to those who can hack it. Zer0Day Xpl01t puts you in the role of a hacker-for-hire, taking contracts, building your toolkit, and climbing the ranks of the digital underground through interactive mini-game puzzles that simulate real hacking techniques.

<!-- SCREENSHOT: Hero shot - DeckView home screen showing the app grid, stats header, and darknet ticker with the Ghost (green) theme active -->
![Home Screen](screenshots/home-screen.png)

## Features

### Custom Windowing System

Every tool in your arsenal runs as a floating window on your hacking deck. Drag, resize, minimize, and layer multiple apps simultaneously -- just like a real operating system. On iPhone, apps expand to fill the screen. On iPad, windows float freely with full drag-and-resize support.

<!-- SCREENSHOT: iPad showing 2-3 overlapping app windows (e.g., Node Connection, Messages, and Terminal) demonstrating the floating window system -->
![Windowing System](screenshots/windowing-system.png)

### Five Playable Characters

Choose your identity. Each character transforms the entire UI with distinct color palettes, fonts, animations, and visual effects.

| Character | Identity | Visual Style |
|-----------|----------|-------------|
| **Ghost** | Freelance Hacker | Phosphor green on black, monospace font, grid overlays |
| **Mole** | Corporate Insider | Corporate blue on white, Helvetica, clean glass aesthetic |
| **Radical** | Resistance Fighter | Revolutionary red on black, bold condensed font, punk aesthetic |
| **Turncoat** | Ex-Security | Amber neon with cyan accents, Futura font, noir rainfall effects |
| **Glitch** | AI-Touched | Neon pink with electric purple, digital distortion effects |

<!-- SCREENSHOT: Side-by-side comparison showing the same screen (DeckView or a mini-game) under 2-3 different character themes, e.g., Ghost vs Radical vs Glitch -->
![Character Themes](CharacterCollage.png)

### 30 Mini-Games Across 7 Tiers

Your hacking toolkit grows as you level up and earn DigiCreds. Every mini-game is a distinct puzzle mechanic -- no two play alike.

**Starter Pack** (Free)
- **Memory Sequence** -- Pattern replication training
- **Tumbler Crack** -- Audio-based safe cracking
- **Wire Splice** -- Connection routing puzzle

**Basic** (500-1,000 Dc)
- **Guard Pattern** -- Stealth timing analysis
- **Log Parser** -- Pattern recognition in data streams
- **Dumpster Dive** -- Data scavenging utility
- **Hash Collision** -- Cryptographic brute force

**Intermediate** (2,000-3,500 Dc)
- **Firewall Match** -- Firewall bypass puzzle
- **Signal Hijacking** -- Frequency interception
- **Wiper Protocol** -- Priority data destruction
- **Honeypot Defense** -- Trap detection and analysis

**Advanced** (5,000-7,500 Dc)
- **Packet Surfing** -- Rhythm-based packet injection
- **Blackout Window** -- Power grid timing exploit
- **Phishing Campaign** -- Multi-target email exploitation
- **API Exploit** -- Endpoint vulnerability scanner
- **Circuit Trace** -- Visual path analysis
- **Social Engineer** -- Psychological manipulation suite

**Elite** (10,000-15,000 Dc)
- **Drone Override** -- Vehicle hijacking system
- **Deepfake Call** -- Voice impersonation suite
- **AI Jailbreak** -- AI constraint manipulation
- **Corporation War** -- Corporate warfare simulator
- **ICE Programmer** -- Visual security coding interface
- **Memory Implant** -- Memory reconstruction system

**Legendary** (25,000+ Dc)
- **Neural Interface** -- Direct brain-computer interface

<!-- SCREENSHOT: Grid/collage of 4-6 different mini-games in action, showing gameplay variety (e.g., Node Connection path-finding, Port Scanner rhythm lanes, Password Cracker brute force, Social Engineer dialogue tree, Camera Loop CCTV feed, Signal Hijacking waveform) -->
![Mini-Games](screenshots/mini-games-collage.png)

### Mission System

Take contracts from anonymous fixers, corporate insiders, and resistance contacts. Each mission chains multiple mini-games into a hack sequence with narrative context, mid-operation updates, and branching outcomes.

<!-- SCREENSHOT: The Contracts view showing available missions with difficulty ratings, or the Mission Runner view mid-sequence showing stage progression -->
![Missions](screenshots/missions.png)

### Inter-App Communication

Your tools work together. Data Mining can discover encrypted records and automatically launch Password Cracker as a subsystem to decrypt them -- then return the results to the original operation. Apps communicate in real-time, just like a real hacking toolkit.

### Progression & Economy

- **30 Levels** of progression with XP-based advancement
- **DigiCreds (Dc)** -- Earn currency from contracts, spend it on tools
- **Black Market** -- Underground app store with exploits, intel, tools, and temporary boosts
- **Hardware Upgrades** -- Upgrade CPU, RAM, Storage, Cooling, Network, and Battery

<!-- SCREENSHOT: The Black Market view showing purchasable items/apps with prices and rarity indicators, OR the Hardware Upgrades view showing component upgrade cards -->
![Black Market](screenshots/black-market.png)

### Reputation & Heat

Build your reputation across four factions -- **Underground**, **Corporate**, **Public**, and **Ghost** -- while managing heat levels with four megacorporations: **MegaCorp**, **OmniCorp**, **Cyberia**, and **DataDyne**. Your choices shape which contracts become available and how the world reacts to you.

### Darknet Feed

A live-scrolling ticker on your home screen delivers underground chatter, mission foreshadowing, and world-building flavor text. Dive deeper in the full Darknet app to browse the complete feed.

<!-- SCREENSHOT: The Darknet Feed view showing scrolling cyber-chatter messages -->
![Darknet Feed](screenshots/darknet-feed.png)

### Terminal

A command-line interface for direct system interaction, complete with standard commands and hidden capabilities for those who know where to look.

<!-- SCREENSHOT: Terminal view showing green-on-black command prompt with some command output -->
![Terminal](screenshots/terminal.png)

## Tech Stack

- **SwiftUI** -- Declarative UI framework
- **SpriteKit** -- Used for particle effects and animations
- **SF Symbols** -- System iconography throughout
- **JSON-driven missions** -- Mission content defined in data files for easy expansion
- **Singleton architecture** -- Centralized state management with observable objects

## Requirements

- iOS 17.0+
- Xcode 15.0+

## Architecture

```
Zer0Day Xpl01t/
├── Models/          # Data models, player state, mission structures
├── Views/           # All SwiftUI views (30 mini-games + system apps)
├── ViewModels/      # View models for complex mini-games
├── Managers/        # Singleton managers (missions, leveling, audio, etc.)
├── Theming/         # Character themes, glitch effects, shared components
├── Game Logic/      # Base game logic, conversation tree builder
├── Utilities/       # App info provider, extensions
└── Assets.xcassets/ # Icons, backgrounds, camera loop stills
```

## License

All rights reserved. This repository is provided for preview purposes only.
