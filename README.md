[README.md](https://github.com/user-attachments/files/33406985/README.md)
# 🔥 THROUGH HELL

Un **DOOM-clone en un solo archivo HTML**: raycaster 3D con JavaScript vanilla, cero dependencias, cero build. Ábrelo y desciende 10 niveles de horror, cada uno con su ambiente y sus monstruos.

```sh
# sin instalación, sin build:
open index.html        # o arrástralo a tu navegador
```

## 🎮 Jugar

Pulsa **DESCEND**. Mata a **todos** los monstruos del nivel, sigue la brújula `◈ EXIT` hasta el **portal morado** y pulsa **E** para descender. Repite 10 veces. Sobrevive al **REY PÁLIDO**.

## ✨ Features

- 🔫 **Raycaster DDA** a 480 rayos, texturas procedurales, niebla por distancia, linterna con viñeta
- 👹 **10 ambientes únicos**, cada uno con muros, luz, niebla, sangre, mensajes y monstruos propios: aliens, zombis, demonios, sombras, ahogados, autómatas, espectros, vendados, momias… y el Rey
- 🚶 **Monstruos articulados**: ciclos de caminar de 4 frames, persecución implacable con rodeo de esquinas
- 🛒 **Economía + tienda (B)**: los kills dan monedas; compra AR, UZI, pistolas dobles, sniper y hacha arrojadiza
- 🟣 **Portal de salida** sellado hasta el último kill, con aura visible, baliza 3D flotante y brújula de distancia
- 🔊 **Audio sintetizado** con WebAudio: escopetazos por capas de ruido, gritos lejanos, drones, latido a poca vida
- 🔪 Cuchillo de emergencia, hacha arrojadiza, springs de pantalla, partículas de sangre (verde alien incluida)

## 🕹️ Controles

| Tecla | Acción |
|---|---|
| Ratón / swipe (invertido) | Mirar |
| Clic / Espacio | Disparar (mantén con AR/UZI) |
| WASD / flechas, Shift | Moverse / correr |
| 1–6, Q | Armas / rotar |
| B | Tienda (pausa el juego) |
| E | Portal (solo abierto) |
| L / M / R | Fijar puntero / minimapa / reintentar |

## 🗺️ Niveles

| # | Nivel | Huésped |
|---|---|---|
| 1 | Sector 7 Lab | 👽 Aliens |
| 2 | Dead City | 🧟 Zombis |
| 3 | Blood Chapel | 😈 Demonios |
| 4 | Blackwood School | 👻 Sombras |
| 5 | The Sewers | 🌊 Ahogados |
| 6 | The Foundry | 🤖 Autómatas |
| 7 | Hollow Manor | 💜 Espectros |
| 8 | Saint Vex Hospital | 🩹 Vendados |
| 9 | The Sunless Pyramid | 🏺 Momias |
| 10 | Throne of the Beast | 👑 Todos + el REY PÁLIDO |

## 🛠️ Stack & estructura

- `index.html` — **todo el juego**: `LEVELS` (mapas ASCII), `THEMES` (muros, luz, monstruos, sangre), `WEAPONS`, motor, audio y UI
- `README.md` — este archivo
- Sin frameworks, sin assets, sin servidor: Canvas 2D + WebAudio puros

¿Quieres tunearlo? Los mapas son strings (`#` = muro en realidad `1`–`4`, `.` = suelo) y cada tema define sus pintores en `paintMob`/`wallTex`. Añade un nivel copiando un bloque `LEVELS` + su entrada en `THEMES`.

## 🗺️ Roadmap

- [ ] Guardado de progreso (localStorage)
- [ ] Más jefes y armas
- [ ] Modo difícil / permadeath
- [ ] Móvil (joystick táctil)

## 📄 Licencia

MIT — haz lo que quieras con él. Si sobrevives al nivel 10, mencióname en los créditos del infierno.
