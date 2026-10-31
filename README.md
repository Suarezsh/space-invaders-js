# 👾 Space Invaders JS

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Canvas](https://img.shields.io/badge/Canvas_2D-0099CC?style=for-the-badge)
![Sin dependencias](https://img.shields.io/badge/Sin%20dependencias-3fb950?style=for-the-badge)
![License](https://img.shields.io/badge/Licencia-MIT-yellow?style=for-the-badge)

**Recreación del clásico Space Invaders con naves enemigas, disparos, escudos y boss final.**  
Estética neon retro — todo en el navegador, sin instalación.

**[▶ Ver demo en vivo](https://suarezsh.github.io/space-invaders-js)**

</div>

---

## 🎯 ¿Qué es esto?

Una recreación fiel del arcade clásico de 1978, construida desde cero con HTML5 Canvas y JavaScript puro. Incluye todos los elementos del original y agrega un boss final al completar la oleada.

Sin npm, sin frameworks, sin servidor — solo abre `index.html`.

---

## ✨ Características

- 👾 **40 invasores** en formación de 4 × 10, con animación de patas
- 🔫 **Disparos enemigos** — cada columna elige aleatoriamente cuándo atacar
- 🛡️ **4 escudos degradables** — se destruyen bloque a bloque con cada impacto
- 💥 **Boss final** — aparece al eliminar todos los invasores, dispara ráfagas triples y tiene barra de HP
- ⬆️ **Niveles** — cada nivel aumenta la velocidad de los invasores
- ❤️ **3 vidas** — el juego reinicia la posición del jugador al perder una
- 🌟 **Partículas** — explosiones de píxeles al destruir enemigos
- 🎵 **Sonido Web Audio** — efectos de disparo y explosión generados proceduralmente
- 📱 **Touch** — controles táctiles para móvil (desliza para mover, toca para disparar)

---

## 🕹️ Controles

| Acción | Teclado | Touch |
|---|---|---|
| Mover izquierda | `←` o `A` | Deslizar izquierda |
| Mover derecha | `→` o `D` | Deslizar derecha |
| Disparar | `Espacio` | Tocar pantalla |
| Pausar | `P` | — |

---

## 👾 Tipos de enemigos

| Fila | Color | Puntos |
|---|---|---|
| Fila 1 | 🔵 Cian | 10 pts |
| Fila 2 | 🟢 Verde | 20 pts |
| Fila 3 | 🟡 Amarillo | 30 pts |
| Fila 4 | 🟣 Violeta | 40 pts |
| **Boss** | 🔴 Rojo/Naranja | **500 pts** |

---

## 🎮 Mecánicas de juego

### Invasores
Los 40 invasores se mueven en formación horizontal. Al llegar al borde cambian de dirección y descienden una fila. La velocidad aumenta conforme quedan menos invasores vivos.

### Escudos
Los 4 búnkeres están compuestos por bloques individuales con 3 puntos de vida cada uno. Tanto los disparos del jugador como los de los enemigos los dañan. Son la única cobertura del jugador.

### Boss
Al eliminar todos los invasores aparece un boss con 15 HP y barra de vida visible. Se mueve horizontalmente y dispara ráfagas de 3 balas cada 40 frames. Al derrotarlo se avanza al siguiente nivel.

---

## 🖥️ Vista previa

```
┌──────────────────────────────────────────────────┐
│  SCORE: 1240   NIVEL: 2   ❤❤❤   HI: 1240        │
├──────────────────────────────────────────────────┤
│  ·  ·  ·  ·  ·  ·  ·  ·  ·  ·     ← invasores  │
│  ▀  ▀  ▀  ▀  ▀  ▀  ▀  ▀  ▀  ▀                  │
│  █  █  █  █  █  █  █  █  █  █                   │
│  ■  ■  ■  ■  ■  ■  ■  ■  ■  ■                   │
│                                                   │
│  ╔══════════════════════════╗   ← boss           │
│  ║   ◉           ◉         ║                    │
│  ╚══════════════════════════╝                    │
│                                                   │
│  ▓▓▓▓  ▓▓▓▓  ▓▓▓▓  ▓▓▓▓       ← escudos        │
│                    △            ← jugador        │
└──────────────────────────────────────────────────┘
```

---

## 🚀 Uso

```bash
git clone https://github.com/Suarezsh/space-invaders-js.git
cd space-invaders-js

# Abrir directo en el navegador
start index.html        # Windows
open  index.html        # macOS / Linux
```

---

## 📁 Estructura

```
space-invaders-js/
└── index.html    ← Todo en un solo archivo (HTML + CSS + JS)
```

---

## 🛠️ Tecnologías

- **HTML5 Canvas 2D** — renderizado de sprites, partículas y UI
- **Web Audio API** — efectos de sonido generados proceduralmente
- **JavaScript ES6+** — lógica del juego, colisiones y física
- **Google Fonts** — Press Start 2P (fuente pixelada retro)
- **Sin frameworks · Sin librerías · Sin npm**

---

## 📄 Licencia

MIT © [Suarezsh](https://github.com/Suarezsh)
