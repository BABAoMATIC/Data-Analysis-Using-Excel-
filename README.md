# Data-Analysis-Using-Excel-
IFRS Adoption &amp; Financial Performance – Excel Data Analysis This project demonstrates advanced data analysis and financial modeling skills in Excel, using a comprehensive panel dataset of 50 multinational companies (MNCs) across multiple industries, regions, and IFRS adoption timelines.
Key Features
Dataset Size & Structure

700 firm-year observations

Coverage: Multiple industries, regions, and IFRS adoption periods (Pre/Post)

Variables:

Financial metrics (Revenue, Assets, PPE, Net Income, CFO, Receivables)

Accrual-based earnings management measures (ALPHA1, ALPHA2, ALPHA3, NDA, DA)

Change metrics (ΔRevenue, ΔReceivables, scaled assets, etc.)

IFRS adoption year & binary Post-IFRS indicator

Analytical Sheets

Descriptive Statistics – Summary metrics, dispersion, skewness, kurtosis for key variables

Regression Analysis – Model outputs testing relationships between accrual measures and other factors

Correlation Matrix – Identifying potential multicollinearity & relationships between earnings management metrics

ANOVA Single Factor – Testing differences in means across accrual and earnings variables

Panel Data Table – Complete firm-year records for 50 MNCs

Statistical Insights

Significant variability in firm size & performance metrics

Detection of outliers and skewness in earnings distributions

Statistically significant regression results with key predictors

Evidence of differences in discretionary accruals pre- and post-IFRS adoption for certain firms/sectors

Skills Demonstrated
Advanced Excel-based statistical analysis (Descriptive, Regression, ANOVA, Correlation)

Data cleaning & structuring for panel datasets

Financial ratio & metric computation

Visualization-ready outputs for business and academic reporting

Interpretation of statistical results in a corporate finance & accounting context

Potential Use Cases
IFRS adoption impact studies (Difference-in-Differences, Fixed Effects)

Earnings management detection using accrual models

Financial benchmarking across industries and regions

Corporate governance and transparency research
____________________________________________________________________________________________________________________
1. Descriptive Statistics
Covers 700 firm-year observations for variables like Revenue, Total Assets, Receivables, PPE, Net Income, and CFO.

Means:

Revenue: $71B average

Total Assets: $180B average

Receivables: $15.9B average

PPE: $54.25B average

Net Income: $8.29B average

CFO: $9.25B average

Dispersion: High — e.g., Revenue SD ≈ $39.66B, indicating huge size variation across firms.

Skewness & Kurtosis: Many variables are highly skewed & leptokurtic (outliers present), especially Net Income (Kurtosis ≈ 11.76).

Extreme Values:

Max Revenue: $260B, Min: $9.6B

Max Assets: $1.35T, Min: $17.6B

CFO has negative minimum (cash outflow).

2. Regression Output
Regression model estimates:

Fit Statistics:

Multiple R = 0.348, R² = 0.1213 → Model explains ~12% of variance.

Adjusted R² = 0.117 → Minimal overfitting.

Observations: 699

ANOVA:

F-stat ≈ 32.03, p < 2.11×10⁻¹⁹ → overall model is statistically significant.

Coefficients:

Intercept: -67.06 (p=0.233) → not significant.

Var2: -0.02285 (p=0.376) → not significant.

Var3: -0.01506 (p ≈ 3.75×10⁻¹⁰) → highly significant, negative impact.

3. Correlation Matrix (ALPHA variables, NDA, DA)
Strong correlation between ALPHA 3 and NDA: 0.6805 → may indicate potential multicollinearity if both used in regression.

DA correlations are low with all variables (max |r| ≈ 0.083).

ALPHA variables very weakly correlated with each other (near zero).

4. ANOVA Single Factor
Comparing means of ALPHA 1, ALPHA 2, ALPHA 3, NDA, DA:

Between-group differences highly significant (F=94.7, p ≈ 1.38×10⁻⁷⁶).

Group means:

ALPHA 1 ≈ -0.1016

ALPHA 2 ≈ 0.00271

ALPHA 3 ≈ -0.00583

NDA ≈ -0.00211

DA ≈ -960.50 (scale far larger; may distort ANOVA).

5. Panel Data ("Data" Sheet)
Large panel format: Company, Country, Region, Industry, IFRS Adoption Year, Year, Pre/Post IFRS, financials, accrual measures, residuals.

Covers 50 multinational companies (MNCs) from various regions/industries.

Time coverage varies — some pre-2005 adoption, some later (e.g., DBS in 2018).

Variables: raw financials (Revenue, Assets…), changes (DeltaRev, DeltaRec), scaled totals (TA, STA), accrual metrics (InvA1, RevAdj, PPE), and accrual measures (Alpha1, Alpha2, Alpha3, NDA, DA).

PostIFRS Flag marks IFRS adoption period observations.

Initial Observations
IFRS Adoption Effect: Can be tested using this panel (DiD, fixed effects).

Accruals & Earnings Management: ALPHA variables seem to be accrual-based measures; DA/NDA likely discretionary/nondiscretionary accruals — correlation shows NDA & Alpha3 are closely related.

Industry/Country Mix: Broad coverage allows cross-sectional analysis.

___________________________________________________________________________________
Practical screenshots
<img width="1662" height="412" alt="image" src="https://github.com/user-attachments/assets/7b40045e-f4e1-40af-948d-a6680353b303" />

<img width="537" height="331" alt="image" src="https://github.com/user-attachments/assets/388bb00f-8368-44a8-8bb4-8a90d1c75374" />

<img width="162" height="621" alt="image" src="https://github.com/user-attachments/assets/54561178-0c1d-43d1-815e-3dcaa1ef3b05" />
<img width="522" height="165" alt="image" src="https://github.com/user-attachments/assets/a2be9d39-6ee0-4077-8cdf-733cde55e170" />

<img width="166" height="203" alt="image" src="https://github.com/user-attachments/assets/7ad71e57-60b1-4d81-8ed9-48cd8119bd47" />

<img width="505" height="122" alt="image" src="https://github.com/user-attachments/assets/c85f14ca-8d72-4ed5-b38b-4db6541e77b7" />

<img width="740" height="138" alt="image" src="https://github.com/user-attachments/assets/c64b38b0-7e3a-4265-b7a2-893c58edcb61" />

<img width="602" height="307" alt="image" src="https://github.com/user-attachments/assets/0458ff80-6718-4f92-ae76-c495fb7a1db0" />

<img width="610" height="180" alt="image" src="https://github.com/user-attachments/assets/30ac865c-5309-477f-9e7c-282712032985" />

<img width="770" height="182" alt="image" src="https://github.com/user-attachments/assets/f88f65ba-aad5-41f0-a95d-0cc0be961688" />

<img width="590" height="337" alt="image" src="https://github.com/user-attachments/assets/dc29101f-9dde-4b5c-bfc7-fbca6a144523" />
<img width="545" height="336" alt="image" src="https://github.com/user-attachments/assets/602f9784-2179-4a34-8565-eeb97bff21c9" />






