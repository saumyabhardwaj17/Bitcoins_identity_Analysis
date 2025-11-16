# Bitcoin’s Identity: Digital Gold or Speculative Asset?

## By Group 6

This Jupyter Notebook project explores the evolving identity of **Bitcoin (BTC)** by analyzing its price, volume, volatility, correlations, and relationship with traditional assets like **tech equities (QQQ)** and **gold (XAU)**. The aim is to assess whether Bitcoin behaves more like a safe-haven "digital gold" or a speculative, risk-on asset.

---

## Project Structure

- **Jupyter Notebook (`Bitcoin_Analysis.ipynb`)**  
  Contains all the code for data preprocessing, visualization, correlation analysis, rolling volatility, and regression modeling.

- **Excel Data File (`bloomberg.xlsx`)**  
  Contains historical price and volume data for:
  - Bitcoin (`BTC` sheet)
  - Nasdaq ETF (`QQQ` sheet)
  - Gold futures (`XAU` sheet)

---

## Tools & Libraries

- **Python Libraries:**  
  `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `yfinance`, `scikit-learn`

- **Visualizations:**  
  - Log-transformed price trends with dual axes  
  - Faceted volume bar charts  
  - Rolling volatility and correlation plots  
  - Heatmaps for pre- and post-ETF correlation  
  - Macro event highlighting with shaded areas and ETF approval lines  

- **Statistical Analysis:**  
  - Rolling correlations (30-day, 90-day)  
  - Linear regression to quantify BTC sensitivity to tech and gold  

---

## Analysis Steps

1. **Data Preprocessing:**  
   - Load BTC, QQQ, and XAU data from Excel.  
   - Clean column names, convert dates to `datetime`.  
   - Merge datasets on common dates and apply log transformations.

2. **Volume Analysis:**  
   - Visualize BTC, QQQ, and XAU trading volumes over time.  
   - Add horizontal average volume lines for reference.  
   - Observed BTC as highly volatile, QQQ as stable, and Gold as thinly traded.

3. **Volume Correlation Post-ETF:**  
   - Compute log changes in volume and 30-day rolling correlations.  
   - Highlighted that BTC and QQQ volumes move together post-ETF, indicating shared investor behavior.

4. **Price Correlations and Rolling Volatility:**  
   - Split data pre- and post-ETF.  
   - Compute correlation matrices and visualize via heatmaps.  
   - Compute 30-day rolling volatility and show BTC is consistently more volatile than tech and gold.

5. **Rolling Price Correlations with Macro Events:**  
   - Compute 90-day rolling correlations between BTC vs QQQ and BTC vs XAU.  
   - Overlay major macro events (CME launch, COVID crash, Fed rate hikes) and ETF approval.  
   - Observed BTC increasingly moves with tech stocks and remains uncorrelated with gold.

6. **Regression Analysis:**  
   - Linear regression of BTC price against QQQ and XAU.  
   - BTC shows higher sensitivity to tech stocks than gold, reinforcing risk-on behavior.

---

## Key Findings

- **BTC is highly volatile** and speculative compared to QQQ and gold.  
- **BTC correlates strongly with tech stocks** and only weakly with gold.  
- **ETF approval and macro events** have increased BTC’s alignment with risk-on assets.  
- Regression shows **BTC is more sensitive to tech equities** than gold.  

**Conclusion:**  
Bitcoin behaves more like a **speculative, risk-on macro asset** than a traditional safe-haven "digital gold." Its price and volume dynamics are influenced by liquidity, institutional participation, and market sentiment.

---

## Usage

1. Open `Bitcoin_Analysis.ipynb` in Jupyter Notebook or JupyterLab.  
2. Ensure `bloomberg.xlsx` is in the same directory.  
3. Run the notebook sequentially to reproduce all plots and analysis.

---

## Visualizations

- Log-transformed BTC, QQQ, and Gold prices with dual y-axis.  
- Facet grid for BTC, QQQ, and Gold volumes with average lines.  
- Rolling 30-day volatility plot with ETF marker.  
- 90-day rolling correlations with macro event shading.  
- Pre- and post-ETF correlation heatmaps.  
- Regression outputs for BTC vs QQQ and BTC vs Gold.  

---

## References

- Historical data sourced from Bloomberg and Yahoo Finance (`yfinance`).  
- Macro events: CME futures launch, COVID-19 crash, Fed rate hikes, ETF approval.

---

## Author

**Group 6 - MAM, LBS'26**  
Analysis conducted as part of a project exploring Bitcoin’s identity relative to traditional assets.
