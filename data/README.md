# Data Sources & Access

This folder does not contain raw `.csv` or `.xlsx` files. To ensure absolute reproducibility and to avoid large file hosting, all macroeconomic time series are queried and downloaded automatically at runtime using the [`ipeadatar` package API](https://github.com/ipea/ipeadatar).

Below is the documentation for the datasets manipulated in this research. Reviewers can verify the exact metadata for any series directly in the R console using the `ipeadatar::metadata("SERIES_CODE")` function, or by searching the series code at the [Ipeadata Official Portal](http://www.ipeadata.gov.br/).

### Demographic Dependency Ratio (DDR)
* **API Series Code:** `ADH12_RAZDEP`
* **Original Source:** IBGE (Demographic Census & PNAD) via Atlas of Human Development.
* **Description:** Proportion of the inactive population (0-14 and 65+ years) relative to the potentially productive population (15 to 64 years).

### Brazilian Labor Productivity
Calculated in the script as the ratio between Real GDP and Total Employed Persons.
* **Real GDP (Numerator):** 
  * API Series Code: `SCN10_PIBP10` 
  * Source: IBGE - System of National Accounts (SCN).
* **Employed Persons (Denominator):** 
  * API Series Code: `PAN_PO` 
  * Source: IBGE - Continuous National Household Sample Survey (PNAD Contínua).

### Global Benchmarks
* **Original Source:** World Bank Open Data (World Development Indicators).
* **Description:** GDP per person employed for the control group (Vietnam, Poland, South Korea, Chile).
* **Reference Link:** [World Bank Data Portal](https://data.worldbank.org/indicator/SL.GDP.PCAP.EM.KD)
