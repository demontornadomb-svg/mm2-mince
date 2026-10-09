# MM2 Mince 🪙

Local Windows experiment that detects coins in Murder Mystery 2 and attempts to guide the character toward them. Vision and input processing run locally; Codex or ChatGPT is not required while using it.

**Version 3.4.0 is experimental.** Obstacle routing and actual coin pickup are not guaranteed. The latest changes passed offline checks, but were not retested in a live Roblox round.

## Download

Open **Releases**, choose **3.4.0**, and download **MM2-Mince-3.4.0.exe** from **Assets**. The “Source code (zip)” download contains the repository files, not the packaged application.

The program is free to download. The EXE includes the required Python runtime and libraries, so they do not need to be installed separately. It is intended for 64-bit Windows; other computers have not been verified.

## Usage

1. Start the EXE. Automatic movement is disabled when the app opens.
2. Open Murder Mystery 2, keep the camera behind the character, and close the chat and menus. Classic mode without Shift Lock is recommended.
3. Start collection with the button in the app or with **F8** while the game is focused.
4. **F8** toggles collection and pause. **F9** or **Esc** stops control. Switching to another window also stops automatic movement.

The manual training tab can save your own screenshots and observed inputs. Recording gameplay does not create a complete learned map or automatically replace the movement rules. Records are stored locally in the app's user data, not inside the EXE.

## Changes in 3.4.0

- The selected coin stays the target while the controller makes a short, verified obstacle detour.
- Side movement stops when a passage is aligned; a fresh frame then checks forward progress.
- Repeated or stale frames cannot confirm a successful bypass.
- A camera change invalidates the previous short-term obstacle context.
- The preview shows the current detour waypoint when navigation supports it.

## Verification and limitations

The project passed **342 automated tests**. An offline smoke test for the packaged EXE verified sample coin detection, controller initialization, and creation of a hidden test window. This does not prove reliable walking, wall avoidance, or coin pickup in a live game.

In a comparison of 22 extended model routes, both the previous and current version reached the target distance in 17 cases. The model uses more reliable prompts than real screen recognition, so the program is still an experimental navigator and may fail or get stuck on some maps.

The EXE is unsigned. Windows may block it; do not disable Defender or other security protections to run it. Use **SHA256SUMS.txt** to check that the downloaded file matches this release; a matching hash alone is not a guarantee of safety.

## Privacy

Game-screen processing runs on the local computer. The app does not require Roblox credentials. The public release contains no personal training sessions, settings, or original videos. The EXE includes a sample game frame and coin image references.

## Support the project ⭐

If you find the project useful, please give the repository a **Star ⭐**. It is a free way to show support on GitHub. You can also open an **Issue** with the app version and a short description of a problem. Do not include passwords, tokens, or private recordings.

## Relationship to the game

This is an unofficial personal project and is not affiliated with Roblox or the creators of Murder Mystery 2. Game names and image material belong to their respective owners. Check the rules of the game before using any automation.
