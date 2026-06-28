# Arbitrum L2 — Landing Page & Interactive Web3 Simulator

A premium, interactive single-page web application (SPA) designed to explore Ethereum Layer-2 scaling, core Web3 concepts, real-time market data, and blockchain mechanics.

Designed with a sleek, futuristic dark mode aesthetic, this application acts as an educational portal for anyone looking to understand rollups, Layer-2 scaling, and general blockchain immutability.

---

## 🚀 Features

### 1. **Interactive Block Simulator**
*   **Tamper-Proof Ledger Demonstration:** Visualizes how blocks link together in a chain using cryptographic hashes.
*   **Live SHA-256 Mining:** Custom transaction input fields allow users to mine blocks live. An asynchronous mining loop uses yields to prevent the browser tab from freezing.
*   **Immutability Visualization:** Modifying data in an upstream block immediately invalidates its hash, breaking the sequential chain and demonstrating how distributed ledgers detect tampering.

### 2. **Conceptual Web3 Guide**
*   Four interactive cards and side-by-side comparison tables explaining core concepts:
    *   **Web2 vs. Web3:** Contrasting platforms/centralized databases with user-owned assets and protocol control.
    *   **Ethereum vs. Bitcoin:** Gold standard store-of-value vs. Turing-complete smart contract ecosystem.
    *   **Public/Private Keys:** Demystifying cryptographic keypairs and account signatures.
    *   **Blockchain vs. Databases:** Understanding append-only, decentralized ledger structures vs. standard CRUD operations.

### 3. **Live Crypto Tracker**
*   **Real-time Prices:** Integrates with the CoinGecko Simple Price API to retrieve the current market rates for **Bitcoin (BTC)**, **Ethereum (ETH)**, **Arbitrum (ARB)**, **Solana (SOL)**, and **Polygon (POL)**.
*   **Auto-Sync:** Dynamically pulls and refreshes market data every 60 seconds with an optional manual refresh button.

### 4. **Modern Design System**
*   **Aesthetics:** Sleek grid systems, immersive HSL gradients, glassmorphism layers, and responsive CSS styling.
*   **Micro-Animations:** Beautiful hover transitions, floating 3D-like cubes, active navigation indicators, and page-in routing animations.

---

## 🛠️ Technology Stack

*   **Frontend Library:** [React 18](https://react.dev/) (via unpkg CDN)
*   **Styling & Layout:** [Tailwind CSS](https://tailwindcss.com/) (via CDN)
*   **Transpiler:** [Babel Standalone](https://babeljs.io/) (for in-browser JSX transpilation)
*   **Icons:** [Lucide Icons](https://lucide.dev/)
*   **Cryptography:** Native browser Web Cryptography API (`crypto.subtle.digest`) for computing SHA-256 hashes.
*   **Market Data API:** [CoinGecko API v3](https://www.coingecko.com/en/api)

---

## 📂 Project Structure

```text
├── Arbitrum L2 Site.html              # Core single-page application
├── Arbitrum L2 Site.html.srcmap.json  # Dev source map
├── README.md                           # Documentation
└── screenshots/                        # Captured states of the UI
    ├── home.jpg                        # Homepage screen
    └── multi_mqxi*/                    # Simulated walkthrough steps
```

---

## 💻 Getting Started

Because this project is built using browser CDNs, it requires zero build steps or local package installations. You can run it instantly.

### Option A: Local Browser
Double-click [Arbitrum L2 Site.html](file:///c:/Users/Akshay/OneDrive/Desktop/project/Arbitrum%20L2%20Site.html) to open the file directly in any modern web browser.

### Option B: Local HTTP Server (Recommended)
To run with correct network routes and prevent potential CORS issues with browser APIs, host it locally using a simple HTTP server:

**Using Python:**
```bash
python -m http.server 8000
```
Then visit `http://localhost:8000/Arbitrum L2 Site.html` in your browser.

**Using Node.js (`npx`):**
```bash
npx serve .
```

---

## 📸 Preview Screenshots

Refer to the [screenshots/](file:///c:/Users/Akshay/OneDrive/Desktop/project/screenshots) folder to see previews of the interface, including the Live Market dashboard and the interactive Block Simulator.