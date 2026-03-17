🕹️ PAC-MAN ARCADE: HTML5 Canvas Edition
A high-fidelity, retro-futuristic recreation of the classic 1980s arcade phenomenon. Built entirely with HTML5, CSS3, and Vanilla JavaScript, this project features a custom physics engine, pathfinding AI, and a synthesized Web Audio API system.

✨ Features
🎨 Retro-Futuristic UI
Virtual Arcade Cabinet: A CSS-styled frame featuring a pulsing "Marquee" neon sign and a CRT scanline overlay.

Dynamic Particle System: Real-time bursts and floating score text using a custom class-based particle engine.

Responsive Controls: Support for Keyboard (WASD/Arrows), Touch Swipes, and an interactive Virtual Joystick.

🧠 Intelligent Ghost AI
The game implements a custom A (A-Star) Pathfinding Algorithm* with distinct "personalities" for the ghosts:

Blinky (Red): Direct pursuit.

Pinky (Pink): Ambush logic (targets tiles ahead of the player).

Inky (Cyan): Erratic/Unpredictable movement.

Clyde (Orange): Pursues until close, then retreats to his corner.

Smart State Machine: Ghosts transition seamlessly between HOUSE, EXITING, NORMAL, FRIGHTENED, and RETURNING (eyes only) states.

🔊 Procedural Web Audio
No MP3 files required! All sounds are synthesized in real-time using the Web Audio API:

Square-wave "Waka-waka" dot eating.

Sawtooth-wave death sequences.

Triangle-wave level-clear melodies.

Dynamic background "Siren" that pulses during gameplay.

🗺️ Technical Map Engine
Tile-Locked Movement: Prevents Pac-Man from "sticking" to corners by enforcing pixel-perfect grid alignment.

Tunnel Logic: Seamless horizontal wrapping at row 11.

Procedural Maze Rendering: A sophisticated wall-drawing algorithm that calculates convex and concave corners to create smooth, connected neon borders.

🎮 How to Play
Objective: Eat all dots (.) and Power Pellets (o) to clear the level.

Controls:

PC: Use Arrow Keys or WASD.

Mobile: Swipe on the screen or use the Virtual Joystick at the bottom.

Scoring:

Dots: 10 pts

Power Pellets: 50 pts

Ghosts: 200, 400, 800, 1600 pts (Combo)

Fruits: 🍒(100) → 🍓(300) → 🍊(500) → 🍋(700) → 🍎(1000)

🚀 Installation & Setup
Since this project is built with Vanilla JS, no build tools are required.

Clone the repository:

Bash
git clone https://github.com/yourusername/pacman-arcade.git
Open index.html in any modern web browser.

Note: Most browsers require a user interaction (like clicking "Play") to enable the Web Audio API.

🛠️ Technical Details
Grid Size: 21 Columns × 23 Rows.

Resolution: 420px × 460px (Canvas).

Frame Rate: Optimized for 60FPS using requestAnimationFrame.

Font: Orbitron via Google Fonts.

📜 License
Distributed under the MIT License. See LICENSE for more information.

© 1980 NAMCO (Original Concept) | 2024 Re-imagined by Anthony Mendoza

Sería genial si pudieras:
¿Te gustaría que añadiera una sección de "Roadmap" con futuras mejoras?

¿O quizás una tabla comparando las dificultades de cada nivel?
