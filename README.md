# 🌍 Renewable Energy Trends Analysis

## 📖 Project Overview

This project analyzes global renewable energy trends using a comprehensive dataset covering energy production, investments, policies, and economic factors that shape renewable adoption worldwide. The analysis was conducted as part of a data science challenge to uncover insights about the global transition to clean energy.

## 🎯 Mission

As a data analyst at NextEra Energy, the mission is to explore multi-dimensional renewable energy data and uncover powerful insights about global trends. The analysis addresses key questions such as:
- Which regions are investing most efficiently in renewables?
- How do economic, environmental, and policy factors relate to production levels?
- What drives successful renewable energy adoption across different countries?

## 📊 Dataset Overview

The analysis uses a rich global renewable energy dataset with **2,400 observations** and **31 features** covering:

### 🌍 Basic Identifiers
- **Country** – Country name
- **Year** – Calendar year (YYYY)
- **Energy Type** – Type of renewable energy (Solar, Wind, Hydro, Biomass, Geothermal)

### ⚡ Energy Metrics
- **Production (GWh)** – Renewable energy produced (Gigawatt-hours)
- **Installed Capacity (MW)** – Installed renewable capacity (Megawatts)
- **Investments (USD)** – Total investment in renewables (US Dollars)
- **Energy Consumption (GWh)** – Total national energy use
- **Energy Storage Capacity (MWh)** – Capacity of energy storage systems
- **Grid Integration Capability (Index)** – Scale of 0–1; ability to handle renewables in grid
- **Electricity Prices (USD/kWh)** – Average cost of electricity
- **Energy Subsidies (USD)** – Government subsidies for energy sector
- **Proportion of Energy from Renewables (%)** – Share of renewables in total energy mix

### 🧠 Innovation & Technology
- **R&D Expenditure (USD)** – R&D spending on renewables
- **Renewable Energy Patents** – Number of patents filed
- **Innovation Index (Index)** – Global innovation score (0–100)

### 💰 Economy & Policy
- **GDP (USD)** – Gross domestic product
- **Population** – Total population
- **Government Policies** – Number of policies supporting renewables
- **Renewable Energy Targets** – Whether national targets are in place (1 = Yes, 0 = No)
- **Public-Private Partnerships in Energy** – Number of active collaborations
- **Energy Market Liberalization (Index)** – Scale of 0–1

### 🧑‍🤝‍🧑 Social & Governance
- **Ease of Doing Business (Score)** – World Bank index (0–100)
- **Regulatory Quality** – Governance score (-2.5 to 2.5)
- **Political Stability** – Governance score (-2.5 to 2.5)
- **Control of Corruption** – Governance score (-2.5 to 2.5)

### 🌿 Environment & Resources
- **CO2 Emissions (MtCO2)** – Emissions in million metric tons
- **Average Annual Temperature (°C)** – Country's average temperature
- **Solar Irradiance (kWh/m²/day)** – Solar energy availability
- **Wind Speed (m/s)** – Average wind speed
- **Hydro Potential (Index)** – Relative hydropower capability (0–1)
- **Biomass Availability (Tons/year)** – Total available biomass

## 🔍 Key Findings

### Investment Efficiency Analysis
- **China, Japan, and India** lead in investment efficiency (GWh produced per USD invested)
- Investment efficiency shows the strongest positive correlation with production levels
- Efficient investment strategies are more important than raw investment totals

### Production Trends
- Renewable energy production shows **temporal growth** over the years
- **Hydro and Wind** energy types show substantial production globally
- **Solar and Biomass** also contribute significantly to the renewable mix

### Correlation Insights
**Positive Correlations with Production:**
- Investment Efficiency
- Average Annual Temperature
- Public-Private Partnerships in Energy
- Renewable Energy Targets
- Solar Irradiance
- Electricity Prices
- Proportion of Energy from Renewables
- Wind Speed
- Hydro Potential
- Innovation Index
- Energy Market Liberalization

**Negative Correlations with Production:**
- CO2 Emissions
- Energy Consumption
- Renewable Energy Patents
- Political Stability
- Investments (USD)
- Population
- Control of Corruption
- Regulatory Quality
- Ease of Doing Business
- Biomass Availability
- Energy Storage Capacity
- Energy Subsidies
- Grid Integration Capability
- R&D Expenditure
- Installed Capacity (MW)
- GDP
- Government Policies

## 📈 Statistical Analysis

### Multiple Linear Regression Results
- **R-squared: 0.017** – Model explains ~1.7% of variance in Production (GWh)
- **Year** (p < 0.001): Positive and significant, confirming temporal growth
- **Average Annual Temperature** (p = 0.003): Positively associated with production
- **Investment Efficiency** (p ≈ 0.068): Marginally significant

### Model Limitations
- Low explanatory power suggests complex, non-linear relationships
- High condition number (3.43e+17) indicates multicollinearity among predictors
- Model useful for hypothesis testing despite low R²

## 🎨 Visualizations

The project includes:
- **Investment Efficiency by Country** - Bar chart showing GWh/USD efficiency across nations
- **Correlation Matrix Heatmap** - Comprehensive view of feature relationships
- **Production Trends** - Time series analysis by energy type and country

## 📁 Project Structure

```
workspace 3/
├── data/
│   └── Training_set_augmented.csv    # Main dataset (2,400 observations, 31 features)
├── notebook.ipynb                    # Complete analysis notebook
├── investment_efficiency_by_country.png  # Visualization output
└── README.md                         # This file
```

## 🛠️ Technical Stack

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Basic plotting
- **Seaborn** - Statistical data visualization
- **Statsmodels** - Statistical modeling and regression analysis
- **Tabulate** - Data table formatting

## 🚀 Getting Started

1. **Clone or download** the project files
2. **Install dependencies** (if needed):
   ```bash
   pip install pandas numpy matplotlib seaborn statsmodels tabulate
   ```
3. **Open the notebook** in Jupyter or your preferred environment:
   ```bash
   jupyter notebook notebook.ipynb
   ```
4. **Run the analysis** cells to reproduce the findings

## 📋 Data Requirements

The analysis requires the `Training_set_augmented.csv` file located in the `data/` directory. The dataset contains:
- **2,400 rows** of observations
- **31 columns** of features
- **No missing values** (complete dataset)
- **Mixed data types** (categorical and numerical)

## 🎯 Policy Recommendations

Based on the analysis:

1. **Focus on Investment Efficiency** - Countries should prioritize efficient use of renewable energy investments rather than simply increasing spending
2. **Leverage Natural Resources** - Temperature and renewable resource availability (solar, wind, hydro) significantly impact production
3. **Strengthen Public-Private Partnerships** - These show positive correlation with production levels
4. **Set Clear Renewable Energy Targets** - Countries with targets show better performance
5. **Consider Non-Linear Relationships** - Future analysis should explore more sophisticated modeling approaches

## 🔬 Future Work

The analysis suggests several areas for further investigation:
- **Non-linear modeling** (Random Forests, Time Series, Panel Data Models)
- **Interaction effects** between variables
- **Time-lag effects** not captured by static regression
- **Country-specific policy analysis**
- **Technology-specific efficiency comparisons**

## 📄 License

This project is for educational and analytical purposes. The dataset and analysis are intended to provide insights into global renewable energy trends.


This project was developed as part of a data science challenge. For questions or suggestions about the analysis, please refer to the notebook documentation.

---

*"The race to net-zero emissions is on! As the world battles climate change and rising energy demands, renewable energy is taking center stage."* 🌱⚡ 
