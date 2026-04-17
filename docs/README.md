# ReshEge Helper

[English](./README.md) | [Русский](../README_ru.md)

ReshEge Helper is a userscript that enhances the ReshEge game interface by adding a modern menu, match history, leaderboard, and customization options.  
Additionally, a separate ad‑blocking script is provided to remove intrusive advertisements and anti‑adblock warnings across the entire sdamgia.ru domain.

## ✨ Features

*   Convenient side menu (game only)
*   Leaderboard viewer
*   Match history with detailed error breakdown
*   Light and dark theme support
*   Smooth and fast interface
*   Connection status indicator
*   Extensible functionality
*   **Ad‑blocking companion script** – hides ads and anti‑adblock popups on all pages

## 🛠️ Installation

You need a userscript manager such as **Tampermonkey** or **Violentmonkey** to use these scripts.  
**Two separate scripts are provided:** one for the game enhancements and one for ad removal. Install both for the full experience.

### Step‑by‑step guide:

1.  **Install a userscript manager:**
    *   **Tampermonkey:** [Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) | [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
    *   **Violentmonkey:** [Chrome Web Store](https://chrome.google.com/webstore/detail/violentmonkey/jinjaccalgkegednnccohejagnlnfdag) | [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/violentmonkey/)

2.  **Open the manager's dashboard.** Usually accessible via the extension icon in the browser toolbar.

3.  **Create a new script for the game helper:**
    *   In Tampermonkey click `➕` (Create a new script).
    *   In Violentmonkey click `+` (Create a new script).

4.  **Install `ege_game.js`:**
    *   Open the [ege_game.js](https://github.com/Danex-Exe/ege-game/blob/main/ege_game.js) file in the repository.
    *   Click the `Raw` button to view the source code.
    *   Copy all the code (Ctrl+A → Ctrl+C).
    *   Go back to the manager's editor, select all content (Ctrl+A), and paste the copied code (Ctrl+V).
    *   Save the script (Ctrl+S or `Save & Close`).

5.  **Create a new script for the ad cleaner:**
    *   Repeat step 3 to create another new script.

6.  **Install `ads_cleaner.js`:**
    *   Open the [ads_cleaner.js](https://github.com/Danex-Exe/ege-game/blob/main/ads_cleaner.js) file in the repository.
    *   Click the `Raw` button, copy all code.
    *   Paste it into the new script editor and save.

7.  **Verify the installation:**
    *   Go to the game page [«Hold the Line»](https://ege.sdamgia.ru/game.htm).
    *   A **«MENU»** button should appear on the left side of the screen (from `ege_game.js`).
    *   Browse any other page of the site (e.g., catalog or test) – advertisements and the “Disable adblock” warning should be gone (from `ads_cleaner.js`).
    *   Done! You have successfully installed both ReshEge Helper components.

## 📖 Usage

### Game Helper (`ege_game.js`)

Once installed, a **«MENU»** button appears in the interface **only on the game page**. Click it to open the side panel.

Through the panel you can:

*   **Leaderboard:** View top players.
*   **History:** Detailed breakdown of past matches.
*   **Settings:** Switch between light and dark theme.

### Ad Cleaner (`ads_cleaner.js`)

This script runs automatically on every page of the `sdamgia.ru` domain. It hides:

*   Yandex Direct ad blocks
*   Anti‑adblock warning popups
*   Other promotional elements

No configuration is required – it works silently in the background.

## 📜 Match History

Match history displays information about past games: opponents, rating changes, and time. A detailed error breakdown for each task is also available.

## 🎨 Themes

Both light and dark themes are available. The chosen theme is saved automatically.

## ⚙️ Architecture

The project is built around a modular menu management system responsible for rendering the interface and navigation. Data is loaded dynamically and displayed in the UI.  
The ad cleaner is a lightweight, standalone script that intercepts ad requests and hides specific DOM elements without interfering with the game helper.

## 🧩 Extending

The script can be extended by adding new elements and functions without modifying the core logic.  
The ad cleaner can be adjusted by editing its CSS selector list.

## 🐛 Debugging

Information about the script's operation is available in the browser console (F12 → Console).

## 📄 License

[MIT](../LICENSE)