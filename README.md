# Climate Anomaly

A web tool for computing rainfall and temperature anomaly indices from your own climate data, developed at the ICAR-Indian Agricultural Statistics Research Institute (ICAR-IASRI), New Delhi.

**Live site:** https://pushkarbora.github.io/climate-anomaly/

## What it computes

| Group | Indices |
|---|---|
| Rainfall indices | RAI (van Rooy, 1965), MRAI and SRAI (Ekpetere, 2025), SSPI (Raziei, 2021), SPI (McKee et al., 1993) |
| Anomalies (rainfall, Tmax, Tmin, Tavg) | Standardised anomaly (z-score), deviation from mean, percentage departure |
| Climatology | Baseline mean and standard deviation for every location × calendar month |
| Classes | Dry–wet or cool–warm class for each index; IMD categories for rainfall % departure |

Every index is computed per location and calendar month, against a baseline period you choose: the full record, the last or first N years, or any custom range (for example the WMO 1991–2020 normal).

## How to use

1. Open the live site and go to **Model**.
2. **Upload Data**: a CSV or Excel file (monthly, daily or annual; one row per location, or one column per location).
3. **Match Columns**: confirm which column is the location, year, month (or date) and each variable.
4. **Baseline Period**: choose the reference years for rainfall and temperature.
5. **Indices**: select the indices and press **Compute indices**.
6. On the **Results** page, explore the charts and tables, download the results and climatology as CSV, or print a report.

All computation runs in the browser. Uploaded data is never sent to a server.

## Run locally

Download this repository and open `index.html` in any modern browser. No installation is needed. An internet connection is only needed for web fonts and for reading Excel files; CSV files work offline.

## Developers

- **Dr. Ranjit Kumar Paul**, ICAR National Fellow, ICAR-IASRI, New Delhi
- **Dr. Md Yeasin**, Scientist, ICAR-IASRI, New Delhi
- **Pushkar Bora**, Junior Research Fellow, ICAR-IASRI, New Delhi

## How to cite

Paul, R. K., Yeasin, M., & Bora, P. (2026). *Climate Anomaly: A web tool for rainfall and temperature anomaly indices* [Web application]. ICAR-Indian Agricultural Statistics Research Institute, New Delhi.

## References

- Ekpetere, K. O. (2025). Development and evaluation of the modified and standardized rainfall anomaly indices for extreme variability analysis. *Journal of Environmental Management, 375*, 124160. https://doi.org/10.1016/j.jenvman.2025.124160
- McKee, T. B., Doesken, N. J., & Kleist, J. (1993). The relationship of drought frequency and duration to time scales. *Proceedings of the 8th Conference on Applied Climatology*, 179–184.
- Raziei, T. (2021). Revisiting the Rainfall Anomaly Index to serve as a Simplified Standardized Precipitation Index. *Journal of Hydrology, 602*, 126761. https://doi.org/10.1016/j.jhydrol.2021.126761
- Raziei, T. (2023). Improving the normalization procedure of the simplified standardized precipitation index (SSPI) using Box–Cox transformation. *Stochastic Environmental Research and Risk Assessment, 37*, 925–951. https://doi.org/10.1007/s00477-022-02317-9
- Thom, H. C. S. (1958). A note on the gamma distribution. *Monthly Weather Review, 86*(4), 117–122.
- van Rooy, M. P. (1965). A rainfall anomaly index independent of time and space. *Notos, 14*, 43–48.
- World Meteorological Organization. (2017). *WMO guidelines on the calculation of climate normals* (WMO-No. 1203).
