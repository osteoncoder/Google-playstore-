# Google Play Store Data Analysis - Bubble Chart Project

## Project Overview
This repository contains a comprehensive data analytics and visualization project focusing on Google Play Store application data. The project filters, cleans, and localizes specific app categories, displaying an interactive bubble chart that strictly updates and renders during a live operational time window.

## Data Cleaning & Transformation Processes
- **Dataset Integration**: Successfully loaded and matched clean structured metrics from `app_dataset`.
- **Target Category Filtering**: Retained only applications belonging to specified operational domains: *Game, Beauty, business, commics, communication, Dating, Entertainment, social, and event*.
- **Strict Numeric Filtering**: 
  - Filtered applications with a **Rating strictly greater than 3.5**.
  - Isolated high-engagement rows where **Reviews > 500**.
  - Ensured data popularity thresholds with **Installs > 50,000**.
  - Cleansed text formats (e.g., stripping the 'M' suffix from sizes) to ensure valid numeric data types.
- **Sentiment Boundary**: Kept applications with a text-sentiment subjectivity ratio **greater than 0.5**.
- **String Exclusions**: Filtered out any application containing the letter **'S'** or **'s'** anywhere within its name (e.g., automatically eliminating *Subway Surfers* and *Candy Crush Saga*).

## Localization & Visual Mapping
- **Multi-Lingual Category Mapping**:
  - `Beauty` category localized to Hindi: `सौंदर्य (Beauty)`
  - `business` category localized to Tamil: `வணிகம் (Business)`
  - `Dating` category localized to German: `Dating (Deutsch)`
- **Color Coding**: Mapped the `Game` category strictly to a **Pink** hue within the visual ecosystem.

## Live Operational Window Rule
- To enforce real-time dashboard constraints, the dynamic bubble chart logic is architected to execute and display strictly between **5:00 PM and 7:00 PM Indian Standard Time (IST)**. Outside this time range, it safely falls back to a restricted system-alert notice.


## Task 2: Global Installs - Choropleth Map
- **Visualization**: Created an interactive world map using `px.choropleth` to showcase global app distributions.
- **Exclusion Rule**: Filtered out all categories starting with the characters **"A", "C", "G", or "S"**.
- **Top Categories**: Shortlisted the Top 5 app categories based on cumulative volume of installations.
- **Dynamic Threshold Highlight**: Integrated a logic condition to highlight categories where the total number of installs strictly exceeds 1 Million.
- **Operational Window**: Configured system controls so the map executes and displays strictly between **6:00 PM and 8:00 PM IST**.


## Task 3: Total Installs Trend - Time Series Line Chart
- **Visualization**: Rendered an interactive timeline plot showcasing total installation trajectories segmented by operational domains.
- **Strict Title Compliance**: Displays metrics dynamically with operational time window validation tags.
- **String & Categorical Constraints**: 
  - Automatically filtered out any applications starting with target characters **"x", "y", or "z"**.
  - Enforced structured grouping so categories strictly start with **"E", "C", or "B"**.
- **Localized Presentation**: Maintained localized translations across evaluation modules (*सौंदर्य*, *வணிகம்*, *Dating (Deutsch)*).
- **Growth Shading Layer**: Integrated a highlight filter overlay boundary detecting periods where month-over-month growth patterns scale strictly beyond a **20% threshold ratio**.
- **Operational Window Rule**: Configured tracking matrix variables executing visibility parameters exclusively between **6:00 PM and 9:00 PM IST**.


## Task 4: Cumulative Installs Map - Stacked Area Chart
- **Visualization**: Implemented a layered stacked area plot illustrating cumulative multi-category installation volumes over time.
- **Data Filtering Matrix**: 
  - Restructured to evaluate entities holding an average rating baseline of **at least 4.2**.
  - Enforced string metrics filtering out any applications containing numeric values.
  - Restricted scope to structural groups with categories starting with **"T" or "P"**.
  - Isolated heavy operational scales by verifying reviews strictly **greater than 1,000**.
  - Standardized physical metrics limiting processing sizes between **20 MB and 80 MB**.
- **Localization Integration**: Managed localization transformations for target categorical values (*French*, *Spanish*, *Japanese*).
- **Intensity Layer Rules**: Integrated a dynamic shade overlay execution module mapping alpha intensity shifts during structural growth scaling **over 25% month-over-month**.
- **Time Window Constraint**: Restricted system deployment to live tracking windows exclusively operating between **4:00 PM and 6:00 PM IST**.


## Task 5: Top 10 Categories Metric Comparison - Grouped Bar Chart
- **Visualization**: Deployed an interactive grouped bar chart plotting aggregated average ratings and total review counts side-by-side using log-scale transformations.
- **Strict Data Filters**: 
  - Excluded application profiles holding an average rating baseline lower than **4.0**.
  - Isolated heavy-tier deployments by enforcing physical package constraints of **at least 10 MB**.
- **Temporal Alignment**: Structured timeline queries filtering exclusively for applications whose latest deployment log fell under the month of **January**.
- **Time Window Rules**: Integrated operational validation matrices restricting layout visibility strictly between **3:00 PM and 5:00 PM IST**.


### Task 6: Free vs. Paid Analytics (Dual-Axis Matrix Plot)
* **Goal**: Compares the metrics profile of Free vs. Paid models across the Top 3 market domains using a dual-axis presentation format.
* **Primary Y-Axis**: Average Installs represented as clustered bars.
* **Secondary Y-Axis**: Average Revenue displayed as marked scatter lines.
* **Filtering Conditions Enforced**:
  * Excludes applications with fewer than 10,000 installations and revenue $\ge \$10,000$.
  * Required Android version $> 4.0$ and individual file size $> 15\text{MB}$.
  * Content rating strictly restricted to `'Everyone'`, and app name constraints $\le 30$ characters.
* **Time-Window Restriction**: Configured to display during active audit sessions between **13:00 - 14:00 IST** with a built-in fallback validation view mode.
