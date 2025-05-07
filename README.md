#  Dual-Axis Chart: Free vs Paid App Comparison in Top Categories

This project visualizes a **dual-axis bar chart** in a Jupyter Notebook comparing the **average installs** and **average revenue** for **Free** vs **Paid** apps within the **top 3 app categories** by number of installs.

To ensure quality insights and appropriate context, the chart is only **displayed between 1 PM and 2 PM IST**. Outside that window, a placeholder message is shown.

##  Features

 **Dual-Axis Bar Chart**

- **X-axis:** Free vs Paid apps (for each of top 3 categories)
- **Primary Y-axis:** Average Installs
- **Secondary Y-axis:** Average Revenue

 **Data Filters**

The dataset is filtered with strict business logic:

- ✅ **Installs ≥ 10,000**
- ✅ **Revenue ≥ $10,000**
- ✅ **Android version > 4.0**
- ✅ **App size > 15 MB**
- ✅ **Content rating = Everyone**
- ✅ **App name ≤ 30 characters** (includes spaces & symbols)

 **Time-Gated Access**

- The chart appears **only between 1:00 PM – 2:00 PM IST**
- Outside that window, the chart is hidden and a friendly message is displayed.

##  Use Cases

- Analyzing monetization trends between free and paid apps
- Building time-gated dashboards for demos or restricted reporting
- Educational use to learn conditional visualizations in Jupyter
- Data storytelling using dual-axis plotting
  
## Dependencies
-Python
-pandas for data manipulation
-matplotlib or plotly for dual-axis chart
-pytz and datetime for timezone-aware gating

**Example Workflow** (Inside Notebook)
Load dataset

-Filter by:
Installs, revenue, Android version, size, rating, and name length
Identify top 3 categories by total installs
Aggregate by Free vs Paid

-Render chart with:
One axis for average installs
Second axis for average revenue
Check current time in IST:
If between 1–2 PM → Show chart
    Else → Show notice



