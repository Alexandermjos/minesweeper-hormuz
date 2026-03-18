## Minesweeper Hormuz

A maritime-themed Minesweeper game set in the strategic Strait of Hormuz. Navigate the waters, identify naval mines, and ensure safe passage for civilian shipping in this tactical browser-based challenge.

## 🌊 Overview

Minesweeper Hormuz combines the classic logic-based gameplay of Minesweeper with a real-world geographical context. Instead of a generic gray grid, you are operating over a live map of the Persian Gulf, where landmasses (like the Musandam Peninsula and the Iranian coast) are excluded from the play area, creating a unique and irregular board shape.

## 🚀 Features

Geographical Integration: Powered by Leaflet.js, the game board is mapped directly onto the Strait of Hormuz.

Dynamic Grid Generation: The game identifies landmasses using polygon collision detection, automatically disabling cells located on islands or mainland.

Multiple Difficulty Levels:

Easy: 11x18 grid – Perfect for coastal patrols.

Medium: 17x28 grid – Standard operational sweep.

Expert: 23x38 grid – High-stakes naval clearance.

Cyberpunk UI: A high-contrast, neon-cyan interface built with Tailwind CSS and the Orbitron font for a modern naval command center feel.

Integrated Debug Tools: A specialized developer mode to fine-tune landmass coordinates by clicking directly on the map.

## 🛠️ Tech Stack

HTML5 / CSS3: Core structure and custom styling.

Tailwind CSS: Modern utility-first styling.

JavaScript (Vanilla): Game logic and state management.

Leaflet.js: Interactive mapping engine.

CartoDB Tiles: High-visibility map imagery.

## 🕹️ How to Play

Left Click: Reveal a water tile.

Right Click: Place a warning flag 🚩 on a suspected mine.

The Goal: Reveal all water tiles that do not contain mines.

Win Condition: Successfully clear the strait to ensure maritime safety.

Loss Condition: Detonating a mine results in a radar blackout (Game Over).

## 🔧 Deployment

The project is entirely self-contained in a single index.html file, making it perfect for GitHub Pages.

Create a new GitHub repository.

Upload index.html.

Enable GitHub Pages in the repository settings (Settings > Pages).

## 👨‍💻 Developer Tools (Debug Mode)

To improve the accuracy of the landmasses:

Toggle Debug Mode at the bottom of the screen.

The red outlines show the current collision polygons.

Click anywhere on the map to instantly copy the exact [longitude, latitude] coordinates to your clipboard.

Paste these coordinates into the landPolygons array in the source code to update the coastline.

Safe sailing, Commander.
