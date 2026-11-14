<p align="center">
  <img src="assets/banner.svg" alt="Excel and JSON to Mind Map — your data, as a mind map that fits any screen" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/smabdulmueid97/Excel-JSON-Data-to-fully-responsive-mind-map-Converter"><img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" /></a>
  <a href="https://github.com/smabdulmueid97/Excel-JSON-Data-to-fully-responsive-mind-map-Converter"><img alt="D3.js" src="https://img.shields.io/badge/D3.js-v7-F9A03C?style=flat-square&logo=d3.js&logoColor=white" /></a>
  <a href="https://github.com/smabdulmueid97/Excel-JSON-Data-to-fully-responsive-mind-map-Converter"><img alt="No build step" src="https://img.shields.io/badge/build-none-6366F1?style=flat-square" /></a>
  <a href="https://github.com/smabdulmueid97/Excel-JSON-Data-to-fully-responsive-mind-map-Converter/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/smabdulmueid97/Excel-JSON-Data-to-fully-responsive-mind-map-Converter?style=flat-square" /></a>
</p>

<h1 align="center">Excel / JSON → Mind Map</h1>

<p align="center">
  Turn spreadsheet or JSON data into a <b>fully responsive, interactive mind map</b>.<br />
  Plain HTML + JavaScript with <b>D3.js</b> — no build step, no install.
</p>

<p align="center">
  <a href="#-quick-start">Quick start</a> •
  <a href="#-versions">Versions</a> •
  <a href="#-what-it-does">What it does</a> •
  <a href="#-layout">Layout</a>
</p>

---

## What it does

```mermaid
flowchart LR
    A[Excel / CSV data] --> B[JSON tree<br/>data.json]
    B --> C[D3.js tree layout]
    C --> D[Interactive mind map<br/>click to expand, zoom to explore]
```

- **Collapsible nodes** — nodes start collapsed; click to expand one branch, its siblings collapse.
- **Zoom &amp; pan** — mouse-wheel zoom (0.5×–5× in v1) and drag to move around the map.
- **Paste or upload your data** (v3) — paste JSON into the sidebar, or upload a JSON or CSV file, then hit **Run**.
- **Export graph coordinates** (v3) — export the laid-out node positions from the sidebar.
- **Responsive** — the map sizes itself to the browser window.

## 🚀 Quick start

No install, no build. Serve the folder over HTTP (browsers block `d3.json` from `file://`):

```bash
python3 -m http.server 8000
# open http://localhost:8000/index.html
```

Or right-click `index3.html` → **Open with Live Server** (as the original `Readme.md` suggests).

## 🗂️ Versions

Five versions live side by side — each is one HTML page + its own script and stylesheet. Start with **v3**, the most interactive one.

| Version | Files | Notes |
|---|---|---|
| v1 | `index.html`, `script.js`, `style.css` | Loads `data.json`, D3 tree, collapsible nodes, zoom |
| v2 | `index2.html`, `script2.js`, `style2.css` | Second iteration on the same D3 tree |
| **v3** | `index3.html`, `script3.js`, `style3.css` | **Sidebar: paste JSON, upload JSON/CSV, export graph coordinates, resizable panel** |
| v4 | `index4.html`, `script4.js`, `style4.css` | Fourth iteration on the same D3 tree |
| v5 | `index5.html`, `script5.js`, `style5.css` | Fifth iteration on the same D3 tree |

`data.json` and `data.csv` are the sample datasets the pages load.

## 🗂️ Layout

```
Readme.md               # original notes (local run + Live Server)
index.html              # mind map v1 — "Mind Map v1"
index2.html … index5.html
script.js               # v1 logic — loads data.json, D3 tree
script2.js … script5.js
style.css               # v1 styles
style2.css … style5.css
data.json               # sample data (tree)
data.csv                # sample data (flat)
```

## License

No `LICENSE` file in this repo yet — add one to set the terms.
