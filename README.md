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
Sin archivos MP3 externos. Todo el sonido
