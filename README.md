# Table Fog

A lightweight fog-of-war map viewer for running D&D **in person**. One laptop runs it: the GM controls everything on the laptop screen while a second window, on a TV or monitor at the table, shows the players only what they have discovered.

It is a single HTML file. There is nothing to install, no server and no account, and your maps never leave your computer.

## Features

- **Two windows, one laptop.** The GM screen and the player screen stay in sync. Drag the player window to the TV and press F for fullscreen.
- **Line-of-sight fog.** Place a marker for each character or the party. The marker reveals what it can see, stopping at walls and closed doors. Drag it to explore; crossing a wall pauses revealing until you drop it.
- **Explored vs. visible.** Areas the party has seen but can't currently see are shown dimmed and grey on the player screen.
- **Manual fog tools.** Reveal and hide brushes and boxes, plus Reveal all and Hide all. Works on plain images with no walls.
- **Doors.** Click a door to open or close it. Secret doors and see-through gates are supported.
- **Draw your own walls and doors** on any map, snapped to the half-grid.
- **Player view control.** Zoom, pan, rotate 90° and fit the map, or set **1″ grid** to match physical minis on a flat TV. The player view is shown on the GM map as a dashed box.
- **Ping.** Ctrl+click to flash a marker on the player screen ("you hear something here").
- **Named markers** shown on the player screen, or hidden as GM-only.
- **Map sections.** Group maps into sections (for example by adventure) and drag maps between them.
- **Campaign file.** Save everything (maps, walls, fog, markers, settings) to one `.tablefog` file that is kept up to date automatically.
- **Movable panels.** Drag panel titles to rearrange them on either side of the map, and minimise the ones you don't need.

## Supported maps

| Source | What is imported |
|---|---|
| Foundry VTT scene export (`.json`) and its map image | Image, grid, walls and doors |
| Dungeondraft / Universal VTT (`.dd2vtt`, `.df2vtt`, `.uvtt`) | Image, grid, walls and doors (the image is inside the file) |
| Plain image (`.png`, `.jpg`, `.webp`, …) | Image only; set the grid size and draw walls yourself, or use the brushes |

For a Foundry scene, select or drop the `.json` and its image together. If the image is missing, the app asks for it.

## Getting started

1. Open `index.html` (or the app's GitHub Pages address) in **Chrome or Edge**. Other modern browsers work too, but cannot keep a campaign file linked.
2. Click **Add map…** or drop map files onto the window.
3. Click **Open player window**, drag it to the table screen, then click it or press **F** for fullscreen. Allow pop-ups if the browser blocks it.
4. Press **M** and click the map to place a party marker, then drag it to explore.
5. In the Campaign panel, click **Save as…** to create a campaign file so your prep is backed up.

## Controls

| Action | Control |
|---|---|
| Zoom / pan the GM view | Mouse wheel / right-drag, middle-drag or Space+drag |
| Centre the player view on a spot | Shift+click |
| Slide the player view | Shift+drag |
| Zoom the player view | Shift+wheel |
| Ping | Ctrl+click, or the Ping tool |
| Remove a marker | Right-click it |
| Open or close a door | Click it with Select |
| Brush size | `[` and `]` |
| End a wall chain | Esc |
| Undo the last wall | Ctrl+Z |
| Free wall placement (no snapping) | Hold Alt |
| Fullscreen (player window) | F or click |

**Tool keys:** V select · M marker · R reveal brush · H hide brush · T reveal box · Y hide box · P player view · W wall · D door · E erase wall · X ping

**Player screen buttons:** *Freeze* stops sending changes (useful while you prepare something); *Blank* blacks out the player screen.

## Saving your work

- Everything is saved automatically in the browser as you go. That storage belongs to the browser **and** the address the app was opened from, so a copy opened from a different place (another folder, or a website) starts empty.
- **Campaign file:** *Save as…* creates a `.tablefog` file and links it; changes are written to it about two seconds later. After restarting the browser you may need to click **Reconnect** in the Campaign panel to allow saving again.
- *Open…* loads a campaign file (for example on another computer), replacing what is in the browser. *New* starts an empty campaign.
- If the linked file was changed elsewhere, the newer file is loaded. You're asked first if this browser also has unsaved changes.
- In browsers without file linking (Firefox, Safari), *Save as…* downloads a copy instead.

## Tips

- Set **TV diagonal** in the Player screen panel so the **1″ grid** button matches your screen.
- Set **Vision range** in the Fog panel for dark dungeons; 0 means unlimited.
- A hollow door handle means a see-through door (bars or a gate) that never blocks sight.
- A large campaign file in a synced folder (OneDrive, Dropbox) re-uploads on every save.
