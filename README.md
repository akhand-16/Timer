[chronos_readme_walkthrough.md](https://github.com/user-attachments/files/34211689/chronos_readme_walkthrough.md)
# ⏳ Chronos — Aesthetic Precision Time Suite

🌐 Live Website: https://akhand-16.github.io/Timer/


---

Chronos is a minimalist, pitch-black online time suite inspired by the Claude brand aesthetic. It features an ambient fullscreen clock, an interactive countdown timer, a millisecond-precision stopwatch, a customizable Pomodoro focus engine with acoustic bell chimes, and an offline activity analytics dashboard that syncs directly to a file on your computer.

---

## 🧭 Site Walkthrough & Guide

### 1. The Launcher Menu
When you first open the site, you will see a clean, high-contrast launcher with three primary vertical buttons:
* **CLOCK** — Takes you to the ambient fullscreen real-time clock.
* **TIMER** — Opens the mode selector for **Standard Countdown Timer** or **Pomodoro Focus**.
* **STOPWATCH** — Opens the precision millisecond stopwatch.
* **Quick Utilities** (at the bottom):
  * **ANALYTICS (`📊`)** — Inspect your logged sessions and focus charts.
  * **THEME (`🎨`)** — Customize the accent color across the suite.

---

### 2. Fullscreen Ambient Clock
* **Dead-Center Time Display**: Features extra-bold digits showing hours, minutes, seconds, and AM/PM.
* **12H / 24H Toggle**: Switch between formats with a single click.
* **Copy Time**: Click **COPY TIME** to copy the current timestamp to your clipboard.
* **Auto Ambient Mode**: After **10 seconds of inactivity**, all buttons and navigation cleanly fade away, leaving only the glowing clock visible. Move your mouse or tap the screen to bring the controls back.

---

### 3. Standard Countdown Timer
* **Clutter-Free Interface**: No permanent text fields cluttering the screen.
* **Click-to-Set**: Simply click or tap anywhere on the large digits to bring up the time configuration dialog.
* **Quick Presets & Dials**: Select `+1m`, `+5m`, `+10m`, `+25m`, or adjust hours, minutes, and seconds manually.
* **Controls**:
  * **START / PAUSE / RESUME / STOP / RESTART / RESET**
  * When time runs out, a synthesized acoustic bell strikes, and the session is logged to your analytics.

---

### 4. Pomodoro Focus Workflow
1. Click **TIMER** → Select **POMODORO**.
2. **Custom Minute Inputs**: Enter any number of focus minutes (e.g., `25`, `45`, `60`) and break minutes (e.g., `5`, `15`).
3. Click **START POMODORO**:
   * Transitions into a minimal timer view.
   * Auto-fades after 10 seconds of inactivity.
   * When focus time ends, an acoustic chime rings and it **automatically switches into break mode**.
   * When break time ends, a dialog appears asking: *"Do you want to restart?"*
   * Choosing restart begins another session; choosing stop returns you directly to the Pomodoro configuration page.

---

### 5. Precision Stopwatch
* **Millisecond Precision**: Smooth 60 FPS split rendering.
* **Lap Recording**: Hit **LAP** while running to record split and interval lap times in a neat scrollable overlay.
* **Controls**: Full set of Start, Pause, Stop, Lap, Restart, and Reset buttons.

---

### 6. Activity Analytics & Local File Sync
Access via the **ANALYTICS** button or the chart icon in the top header:
* **Interactive Focus Chart**: Visualizes daily focused minutes using Chart.js.
* **Summary Cards**: Displays Total Focus Time, Rest/Break Time, Completed Pomodoros, and Stopwatch Time.
* **Timeframe Filters**: Filter by **All Time**, **Last 3 Days**, **This Week**, or **This Month**.
* **Connect Local File (Chrome/Edge/Brave/Opera)**:
  1. Click **CONNECT LOCAL FILE**.
  2. Choose a file on your computer (e.g., `chronos_activity_data.json`).
  3. Every session is automatically saved directly to your hard drive in real time.
* **Export / Import**: Use **EXPORT** to download your session log as a JSON file, or **IMPORT** to restore your data on any device.

---

### 7. Theme Studio & Sizing Controls
* **Top Header Slider**: Adjust the digit scale dynamically from `0.5x` up to `1.5x` to suit your screen.
* **Theme Studio**:
  * Pick any custom HEX color or choose from curated presets (**Terracotta**, **Sunset Orange**, **Solar Gold**, **Crimson Red**, **Cyber Cyan**, **Emerald**).
  * Preview the theme live on an interactive mock interface before using it.
* **Fullscreen Button**: Located in the top right to toggle true immersive fullscreen mode (`F11`).

---

## 🛠️ Built With
* Single-file architecture (`index.html`)
* [Tailwind CSS](https://tailwindcss.com/) for responsive typography and layout
* [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API) for synthesized acoustic bell chimes (zero external audio files)
* [File System Access API](https://developer.mozilla.org/en-US/docs/Web/API/File_System_API) for local disk synchronization
* [Chart.js](https://www.chartjs.org/) for activity visualization
* [Font Awesome](https://fontawesome.com/) & Google Fonts (*Bebas Neue*, *Space Grotesk*, *JetBrains Mono*)

---

## 📄 License
This project is open source and available under the [MIT License](LICENSE).
