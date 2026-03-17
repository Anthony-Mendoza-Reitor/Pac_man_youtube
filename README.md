# 🕹️ PAC-MAN ARCADE: Edición Neón Retro-Futurista

Una recreación de alta fidelidad del fenómeno clásico de los 80, construida desde cero con **HTML5 Canvas, CSS3 y Vanilla JavaScript**. Este proyecto combina una estética de "gabinete real" con un motor de físicas personalizado, IA de búsqueda de caminos y audio sintetizado.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white)

---

## ✨ Características Principales

### 🎨 Estética de Gabinete Arcade
* **Marquesina Animada:** Un letrero superior con efectos de pulso neón y luces cíclicas.
* **Interfaz de Puntuación:** Panel dedicado para *High Score*, nivel actual y contador de vidas estilo retro.
* **Efecto CRT:** Superposición de líneas de escaneo (scanlines) para imitar los monitores de tubo antiguos.
* **Sistema de Partículas:** Explosiones visuales al comer fantasmas o píldoras de poder.

### 🧠 Inteligencia Artificial Avanzada (A*)
Los fantasmas no se mueven al azar; utilizan el algoritmo **A-Star (A*)** con comportamientos únicos:
* **Blinky (Rojo):** Persecución directa y agresiva.
* **Pinky (Rosa):** Intenta emboscar al jugador apuntando a celdas por delante de su dirección.
* **Inky (Cian):** Comportamiento errático y flanqueo.
* **Clyde (Naranja):** Persigue al jugador pero huye a su esquina si se acerca demasiado.
* **Estados Complejos:** Manejo de estados de "Hogar", "Saliendo", "Asustado" y "Regresando" (solo ojos) tras ser devorados.

### 🔊 Audio Sintetizado (Web Audio API)
Sin archivos MP3 externos. Todo el sonido se genera en tiempo real:
* **Siren:** Un tono oscilante que aumenta la tensión durante el juego.
* **SFX Dinámicos:** Efectos de comer puntos, muerte del jugador y limpieza de nivel generados mediante osciladores cuadrados y de sierra.

---

## 🎮 Cómo Jugar

1. **Objetivo:** Come todos los puntos (`.`) y píldoras de poder (`o`) para avanzar al siguiente nivel.
2. **Controles:**
   - **Teclado:** Flechas de dirección o teclas `WASD`.
   - **Táctil:** Desliza el dedo (swipe) sobre el canvas.
   - **Joystick Virtual:** Haz clic o presiona el joystick en la parte inferior para dirigir a Pac-Man.
3. **Puntuaciones:**
   - **Puntos:** 10 pts
   - **Píldoras de Poder:** 50 pts
   - **Fantasmas:** 200, 400, 800, 1600 pts (Combo)
   - **Frutas:** 🍒(100), 🍓(300), 🍊(500), 🍋(700), 🍎(1000).

---

## 🛠️ Detalles Técnicos

* **Resolución:** Canvas de 420px × 460px (21x23 Tiles).
* **Renderizado de Laberinto:** Algoritmo de trazado de paredes que calcula esquinas cóncavas y convexas para crear bordes redondeados continuos.
* **Movimiento Tile-Locked:** Sistema que garantiza que Pac-Man solo pueda girar cuando está perfectamente alineado con la cuadrícula, evitando bloqueos en las esquinas.
* **Optimización:** Ejecución fluida a 60 FPS mediante `requestAnimationFrame`.

---

## 🚀 Instalación Rápida

No se requieren dependencias ni herramientas de construcción.

1. Clona este repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/pacman-arcade.git](https://github.com/tu-usuario/pacman-arcade.git)
