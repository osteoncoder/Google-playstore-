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
