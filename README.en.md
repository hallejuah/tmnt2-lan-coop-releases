# TMNT 2: Battle Nexus — LAN Co-op

Play **TMNT 2: Battle Nexus (PC, 2004)** together on **two PCs over a local network**.

**By [x23sunder](https://boosty.to/x23sunder/)** · [Русский](README.md)

**[Download v0.3.2 Alpha](https://github.com/hallejuah/tmnt2-lan-coop-releases/releases/download/v0.3.2-alpha/TMNT2-LAN-Coop-v0.3.2-alpha.zip)** · [All releases](https://github.com/hallejuah/tmnt2-lan-coop-releases/releases)

The ZIP contains **one `TMNT2LanLauncher.exe`**. No PS1/CMD scripts or separate DLL installation is required. Each player needs a compatible copy of the game. Mod sources remain private.

This is an **experimental build**. A complete natural two-player campaign has not been validated.

## Features

- Host on PC1 and join from PC2 using IPv4.
- Each PC sends its own local input and uses its own bindings.
- RU/EN launcher with resolution, fullscreen, borderless/windowed modes and VSync.
- RU/EN waiting and connected screens inside the game window.
- Optional top-right **PING / WAIT / FPS** panel.
- Separate **CoopLab** game copy and LAN progress; the regular game and its saves are preserved.
- Host progress and difficulty are agreed at connection; audio, display and controls remain local.
- Loading, timer and result checks with diagnostic session logs.

The original shared camera is retained. **Team health is shared by design in Battle Nexus; scores are separate.**

## Quick start

1. Both PCs need **Windows 10/11**, **.NET Framework 4.8**, compatible PC game copies and the same LAN.
2. Place the same **`TMNT2LanLauncher.exe`** beside **`TMNT2.exe`** on each PC. Use **Browse** if needed.
3. Select local input and display settings before starting. The two PCs may use different resolutions, window modes and VSync settings. Connect gamepads first.
4. **PC1:** Host game. **PC2:** Join game, enter PC1's IPv4 address and connect. Allow the prepared `TMNT2.exe` on the LAN, TCP port **27804**.
5. Choose New game or Continue. At character selection, PC1 presses **Enter**, then PC2.
6. Use arrows to choose and **F/Enter** to confirm. Assign **all four unique turtles**, at least one to each player, then confirm the roster.

Default keyboard movement is **NumPad 8/4/2/6**. Actions follow the game's bindings. A keyboard on one PC and a gamepad on the other are allowed, but physical gamepad validation is incomplete.

See the **[English instructions](INSTALL-EN.txt)** or [Russian instructions](INSTALL-RU.txt).

## Version 0.3.2 and testing

Adds in-game waiting/connected screens that follow the launcher's RU/EN choice, including with the ping panel disabled. Delayed peer connection and cancellation were tested.

Scoped paired tests cover story transitions, character selection/switches, development-triggered defeat and map replay, results, saving and delayed loading. They are not complete natural campaign playthroughs. Full campaign, all checkpoints, Ride courses, tournaments, natural death/respawn and physical gamepads still need manual validation.

For a problem, preserve both session folders using **Logs** on both PCs. Include the level, last action and affected PC in your report.

## Updating and saves

Close both games/launchers and replace the EXE on both PCs. Keep `CoopLab` to retain LAN progress. Use the same launcher version on both computers.

The LAN profile is `CoopLab\tmntsave.dat`. Sessions use the host's progress, with a backup before changing a LAN profile. Regular game saves are not automatically imported.

**[Boosty — news and author support](https://boosty.to/x23sunder/)** · [TMNT 2003 LAN Co-op](https://github.com/hallejuah/tmnt-2003-lan-coop-releases)

This repository provides compiled releases and documentation. Mod source code is not published. GitHub's generated source archives contain only this download page's files. The game is not included. Unofficial project; TMNT and game materials belong to their respective owners.
