# 📊 FYERS Pro Tool – Risk Calculator + OI Spurts

A sleek, professional Tampermonkey userscript that transforms your FYERS trading platform into a power‑trader dashboard. It combines a real‑time risk calculator with live NSE Open Interest (OI) spurts and market breadth data – all in a beautiful glass‑morphism interface.

---

## ✨ Features

### 🧮 Live Risk Calculator
- Automatically extracts **OHLC** data from the chart and computes:
  - **Stop‑Loss (SL)** – `High – Low`
  - **Ideal Quantity** – based on your custom risk amount (`Risk / SL`, rounded down)
  - **“Ideal” Indicator** – warns you when the SL exceeds **1% of LTP** (helpful for identifying tight stops)
- **Live LTP** displayed for quick reference.
- Smooth **pulse animations** on every value update – gives immediate visual feedback.

### 📈 OI Spurts Viewer
- Fetches the **top 20** F&O stocks with the highest percentage change in Open Interest.
- Displays:
  - **Symbol**
  - **% Change** (in OI)
  - **OI Change** (absolute change)
  - **LTP** (Last Traded Price)
- Striped rows and hover effects for better readability.

### 📊 Market Breadth (Advance / Decline)
- Shows **Advance** and **Decline** counts for all securities in the F&O segment – a quick gauge of overall market sentiment.

### 🖥️ Professional Glass‑Morphism UI
- Semi‑transparent backdrop with blur, gold/amber accents for a premium feel.
- Smooth tab switching with width transitions.
- Compact and uncluttered – perfect for active trading sessions.

### 🖱️ Draggable & Persistent
- Drag the panel only by the **⠿ drag** handle – no accidental moves.
- Position and risk amount are saved automatically in `localStorage` – they persist across page reloads.

### ⌨️ Keyboard Shortcut
- Press **`Alt+Q`** to show/hide the panel instantly.

### 🔄 Auto‑Refresh
- Risk data updates **every second** while the chart is open.
- OI and breadth data refresh on demand – just click the **↻** button.

---

## 🚀 Installation

1. Install a userscript manager like **[Tampermonkey](https://www.tampermonkey.net/)** (or Violentmonkey) in your browser.
2. Click the link below to install the script (or copy the source and create a new script manually):
   - **Install from GitHub Raw:** `[https://github.com/yourusername/your-repo/raw/main/fyers-pro-tool.user.js](https://raw.githubusercontent.com/Anshu-paswan/Riskmanager-For-Trader/refs/heads/main/RiskManager.txt)`
3. The script will automatically run on `https://trade.fyers.in/*`.

> **Note:** If you install manually, make sure the script has the required `@match` and `@grant` permissions.

---

## 🧭 How to Use

| Action | How to do it |
|--------|--------------|
| **Switch Tabs** | Click **Risk** or **OI** at the top of the panel. |
| **Adjust Risk Amount** | Type any number in the **₹ Risk** input – the quantity updates live. |
| **Refresh OI** | Click the **↻** button to reload OI spurts and Advance/Decline. |
| **Move Panel** | Grab the bottom‑right **⠿ drag** handle and drag anywhere on the screen. |
| **Hide/Show Panel** | Press **`Alt+Q`** to toggle visibility. |

---

## ⚙️ Configuration

No extra configuration needed – just install and go.  
The script remembers:
- Your preferred **risk amount**.
- The **panel position** on the screen.

---

## 📝 Important Notes

- The script relies on the OHLC data displayed inside the **TradingView chart iframe** on FYERS. Make sure the chart is fully loaded and visible.
- OI and market breadth data are fetched from NSE’s public APIs – a stable internet connection is required.
- This is a **client‑side** tool; all data is processed locally in your browser. No data is sent anywhere.

---

## 🛠️ Development & Customisation

If you'd like to tweak the script:
- Open the userscript in Tampermonkey and edit the code.
- The CSS is inline for easy modification – you can change colours, sizes, or layout.
- For advanced changes (e.g., adding more data), refer to the NSE APIs used:
  - OI Spurts: `https://www.nseindia.com/api/live-analysis-oi-spurts-underlyings`
  - Advance/Decline: `https://www.nseindia.com/api/NextApi/apiClient/marketWatchApi?functionName=getIndicesData&symbol=SECURITIES%20IN%20F%26O`

---

## 📸 Screenshots

*(Add screenshots of the panel in action here – Risk tab, OI tab, dragging, etc.)*

---

## 🤝 Contributing

Found a bug or have a feature request? Feel free to open an issue or submit a pull request.

---

## 📄 License

This project is open‑source and available under the **MIT License**.

---

## 🙌 Credits

- Built for **FYERS** traders.
- Powered by **NSE India** public APIs.
- Crafted with ❤️ by [Your Name/Handle]

---

**Trade smarter, not harder!** 🚀
