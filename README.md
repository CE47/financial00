# 🧵 Terry's Trousers · Executive Profit Simulator

**Strategic Financial Modeling & Profit Growth Calculator** – an executive‑grade single‑page web app for scenario‑based profit simulation, break‑even analysis, full P&L projections (EBITDA, EBIT, Net Income, Cash Flow), and interactive cost structure visualization.

**Live Demo:** [https://ce47.github.io/financial00/](https://ce47.github.io/financial00/)

---

## ✨ Features

- **Full P&L Modeling** – track Revenue, Gross Profit, EBITDA, EBIT, Net Income after tax, and Operating Cash Flow across a 12‑month horizon.
- **Executive Controls** – adjust Unit Price, Units Sold, Variable Cost, Fixed Cash Costs, **Depreciation**, **Tax Rate**, and Monthly Growth Rate with real‑time updates.
- **Scenario Analysis** – switch between *Realistic*, *Optimistic*, and *Pessimistic* assumptions to stress‑test the entire P&L.
- **What‑If Simulator** – apply percentage changes to Price or Volume and instantly see the impact on Net Income.
- **Two Interactive Charts**:
  - **12‑Month P&L Projection** – line chart showing Revenue, Net Income, and Total Costs.
  - **Cost Structure Breakdown** – stacked bar chart visualising Variable Costs, Fixed Cash, Depreciation, and Net Profit per month.
- **Comprehensive KPI Dashboard** – 12 key metrics including Break‑Even point, Margin of Safety, ROI, and effective Tax Rate.
- **Monthly P&L Breakdown Table** – detailed view of all P&L components for each month.
- **Dark Mode** – toggle between light and dark themes for comfortable viewing.
- **Fully Responsive** – works seamlessly on desktop, tablet, and mobile devices.
- **Zero Dependencies** – self‑contained HTML file with Tailwind CSS, Chart.js, and vanilla JavaScript.

---

## 🚀 How to Use

1. **Open the app** – visit [https://ce47.github.io/financial00/](https://ce47.github.io/financial00/) or open `index.html` locally.
2. **Adjust core drivers** – use the sliders to change unit price, monthly units, variable cost, fixed cash costs, depreciation, tax rate, and growth rate.
3. **Apply scenarios** – click the *Realistic*, *Optimistic*, or *Pessimistic* buttons to see how different market conditions affect the entire P&L.
4. **Run What‑If** – drag the Δ Price and Δ Volume sliders to test the effect of price or volume changes on Net Income.
5. **Analyse results** – monitor the KPI cards, interpret the two charts, and review the monthly breakdown table.
6. **Toggle theme** – click the moon/sun icon in the header to switch between light and dark modes.

---

## 🛠️ Technology Stack

- **HTML5** – semantic markup
- **Tailwind CSS** – utility‑first styling with dark mode support
- **Chart.js** – interactive line and bar charts for financial visualisation
- **Vanilla JavaScript** – all logic, calculations, and DOM manipulation
- **Google Fonts (Inter)** – clean, modern typography

---

## 📦 Deployment to GitHub Pages

This app is designed to be deployed as a static site on GitHub Pages. Follow these steps:

1. Fork or clone this repository.
2. Ensure the main file is named `index.html` and placed at the root of the repository.
3. Go to your repository settings → **Pages**.
4. Under *Branch*, select the branch you want to deploy (e.g., `main`) and save.
5. GitHub will provide a URL (typically `https://<your-username>.github.io/<repo-name>/`).
6. That's it – the app is live!

No build step or server required – it runs entirely in the browser.

---

## 🧩 Customisation

### Adjusting Scenario Multipliers

Open the JavaScript block inside `index.html` and locate the `compute()` function. You can modify the `growthMul` and `demandMul` values for each scenario:

    if (scenario === 'optimistic') { growthMul = 1.4; demandMul = 1.25; }
    else if (scenario === 'pessimistic') { growthMul = 0.6; demandMul = 0.75; }

### Changing Chart Colours

The Chart.js datasets are defined in the `updateCharts()` function. Edit the `borderColor`, `backgroundColor`, or `backgroundColor` (for bars) to match your brand.

### Adding More KPIs

Extend the KPI rows in the HTML and update the `render()` function to compute and display additional metrics (e.g., gross margin per unit, inventory turnover, etc.).

---

## 📸 Screenshots

*Add screenshots here to showcase the dashboard.*

> **Tip:** Replace `./screenshot.png` with actual images from your deployment.

---

## 📝 License

This project is open‑source and available under the [MIT License](LICENSE). Feel free to use, modify, and distribute it as you see fit.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Feel free to check the [issues page](https://github.com/ce47/financial00/issues) if you'd like to help.

---

## 🙌 Acknowledgements

- [Tailwind CSS](https://tailwindcss.com/)
- [Chart.js](https://www.chartjs.org/)
- [Inter Font](https://fonts.google.com/specimen/Inter)

---

*Built with ❤️ for strategic financial modelling and executive decision‑making.*
