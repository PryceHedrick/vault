# Vault

**Pokemon TCG Portfolio Tracker with AI-Powered Analytics**

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-3.0-000000?style=flat-square&logo=flask&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

Track your Pokemon TCG collection's market value with real-time pricing, financial analytics, and AI-powered insights.

---

## Screenshots

### Dashboard
![Dashboard](screenshots/dashboard.png)
*Glassmorphism UI with portfolio metrics, AI insights, and daily performance tracking*

### Collection View
![Collection](screenshots/collection.png)
*Top movers display with full collection table showing P&L, cost basis, and item types*

---

## Features

### Portfolio Dashboard
- Real-time portfolio valuation with daily change tracking
- P&L calculations with editable cost basis
- Card vs sealed product breakdown
- Top holdings by value

### AI Insights
- Portfolio health score (0-100)
- Market momentum indicators
- Profit-taking alerts (50%+ gains)
- Loss review warnings (25%+ drops)
- Concentration risk analysis
- Missing cost basis reminders

### Top Movers
- Daily gainers and losers at a glance
- Percentage change tracking
- Quick identification of market movements

### Modern UI
- Glassmorphism design with animated gradients
- Responsive layout for desktop and mobile
- Dark theme optimized for extended use

---

## Quick Start

```bash
# Clone and install
git clone https://github.com/PryceHedrick/vault.git
cd vault
pip install -e .

# Import your collection (Collectr CSV export)
vault import collection.csv

# Fetch current prices
vault update

# Launch dashboard
vault web
```

Open `http://localhost:5000` in your browser.

---

## CLI Commands

| Command | Description |
|---------|-------------|
| `vault import <csv>` | Import from Collectr CSV |
| `vault update` | Refresh prices from API |
| `vault summary` | Terminal portfolio summary |
| `vault list` | List all items with prices |
| `vault web` | Launch web dashboard |
| `vault export` | Export to CSV |

---

## API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/` | GET | Dashboard |
| `/api/analysis` | GET | Portfolio analytics JSON |
| `/api/items` | GET | All items with prices |
| `/api/items/<id>/cost` | POST | Update cost basis |
| `/api/items/<id>/history` | GET | Price history |

---

## Tech Stack

- **Python 3.10+** - Runtime
- **Flask** - Web framework
- **SQLite** - Database
- **Tailwind CSS** - Styling
- **Chart.js** - Visualizations
- **Pokemon TCG API** - Price data

---

## License

MIT License - See [LICENSE](LICENSE) for details.

---

**Built by [Pryce Hedrick](https://github.com/PryceHedrick)**
