# Stagnant Brazil? The End of the Demographic Dividend and the Middle-Income Trap

## Project Overview
This repository contains an empirical macroeconomic analysis investigating Brazil's structural economic stagnation. By crossing demographic trends with labor productivity metrics, this project explores how the exhaustion of the demographic dividend, combined with institutional bottlenecks, has cemented Brazil in the Middle-Income Trap. 

The research was presented as a working paper at the **BRASA Summit Americas (University of Pennsylvania - Oct 2026)**.

## Tech Stack & Methodology
* **Language:** R
* **Libraries:** `tidyverse`, `ggplot2`, `dplyr`, `ipeadatar`, `knitr`, `kableExtra`
* **Data Sources:** 
  * IPEA (Institute for Applied Economic Research) Cloud API
  * IBGE (Continuous PNAD and SCN)
  * World Bank (WDI Benchmarks)
* **Output:** Quarto/LaTeX PDF Document

## Key Findings
1. **The Demographic Turning Point:** The Demographic Dependency Ratio (DDR) formed a clear "U" curve, hitting its historical minimum in 2017. Brazil's demographic window has officially closed.
2. **Productivity Failure:** Since 2013, Brazilian real labor productivity has stagnated around R$ 45,000 annually at constant prices. The economy failed to transition to technology-driven growth.
3. **Global Benchmarking:** Compared to nations like South Korea (+16.9%), Poland (+37.7%), and Vietnam (+81.5%), Brazil was the only analyzed country to experience a contraction (-1.23%) in productivity growth over the last decade.
4. **Institutional Bottlenecks:** Following the frameworks of Baumol and Douglass North, the research attributes this talent misallocation and lack of innovation to high transaction costs and tax complexity.

## Repository Structure
* `/data`: Notes on data acquisition (raw microdata accessed directly via the `ipeadatar` API).
* `/scripts`: R Markdown (`.qmd`) files containing the data wrangling pipelines and regression models.
* `/output`: Rendered PDF report and high-resolution `ggplot2` visualizations.

## Next Steps (Ongoing Research)
* **Sectoral Decomposition:** Utilizing microdata to pinpoint which specific industries are dragging down the national productivity average.
* **Institutional Impact Modeling:** Quantifying the correlation between local transaction costs and the flight of elite human capital ("brain drain").

---
*Developed by **Mateus Pires Teodoro** - Applied Economics (BS) & Mathematics (BS) at the University of Southern Mississippi.*
