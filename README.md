<h1 align="center">SWYNEX Exploratory Data Analysis – Cafe Sales</h1>

<p align="center">
  <strong>SWYNEX Internship – Task 2: Exploratory Data Analysis (EDA)</strong>
</p>

<hr>

<h2>📌 Project Overview</h2>

<p>
This project was completed as part of the <strong>SWYNEX Internship – Task 2: Exploratory Data Analysis (EDA)</strong>.
</p>

<p>
The objective of this task is to explore a cleaned cafe sales dataset, calculate important statistical measures,
identify trends and patterns, detect potential anomalies, and present the findings using Microsoft Excel,
Pivot Tables, and Pivot Charts.
</p>

<h2>🎯 Objectives</h2>

<ul>
  <li>Perform Exploratory Data Analysis (EDA) on the cleaned cafe sales dataset.</li>
  <li>Calculate important descriptive statistics.</li>
  <li>Analyze product-wise sales and revenue.</li>
  <li>Identify payment method and location-wise patterns.</li>
  <li>Analyze monthly revenue trends.</li>
  <li>Detect potential high-value transaction outliers using the IQR method.</li>
  <li>Create Pivot Tables and Pivot Charts.</li>
  <li>Identify useful business insights from the dataset.</li>
</ul>

<h2>📊 Dataset</h2>

<p>
The dataset contains <strong>10,000 cafe transactions</strong>.
</p>

<h3>Dataset Columns</h3>

<ul>
  <li>Transaction ID</li>
  <li>Item</li>
  <li>Quantity</li>
  <li>Price Per Unit</li>
  <li>Total Spent</li>
  <li>Payment Method</li>
  <li>Location</li>
  <li>Transaction Date</li>
  <li>Revenue</li>
</ul>

<p>
The <code>Revenue</code> column is calculated using:
</p>

<p align="center">
  <strong>Quantity × Price Per Unit</strong>
</p>

<blockquote>
<strong>Note:</strong> The main transaction-value statistics in this analysis are calculated using the
<strong>Total Spent</strong> column.
</blockquote>

<h2>🛠️ Tools Used</h2>

<ul>
  <li>Microsoft Excel</li>
  <li>Pivot Tables</li>
  <li>Pivot Charts</li>
  <li>Excel Formulas</li>
  <li>Descriptive Statistics</li>
  <li>IQR-based Outlier Detection</li>
</ul>

<h2>📁 Workbook Structure</h2>

<p>
<strong>Excel Workbook:</strong> <code>cafe_sales_cleaned.xlsx</code>
</p>

<table>
  <thead>
    <tr>
      <th>Worksheet</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>dirty_cafe_sales_Cleaned</code></td>
      <td>Cleaned cafe sales dataset used for EDA</td>
    </tr>
    <tr>
      <td><code>EDA Analysis</code></td>
      <td>Pivot Tables, Pivot Charts, analysis summaries and visualizations</td>
    </tr>
    <tr>
      <td><code>Caluclations</code></td>
      <td>Statistical calculations and supporting metrics</td>
    </tr>
    <tr>
      <td><code>Insights</code></td>
      <td>Final business-oriented insights from the analysis</td>
    </tr>
  </tbody>
</table>

<blockquote>
<strong>Note:</strong> <code>Caluclations</code> is written exactly as it appears in the Excel workbook.
</blockquote>

<h2>📈 Exploratory Data Analysis</h2>

<h3>1. Product Analysis</h3>

<p>
Product-wise quantity and revenue were analyzed to identify the best-performing products.
</p>

<table>
  <thead>
    <tr>
      <th>Product</th>
      <th>Quantity Sold</th>
      <th>Revenue</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Juice</td><td align="right">6,435</td><td align="right">$19,128.50</td></tr>
    <tr><td>Salad</td><td align="right">3,469</td><td align="right">$17,368.00</td></tr>
    <tr><td>Sandwich</td><td align="right">3,428</td><td align="right">$13,792.00</td></tr>
    <tr><td>Smoothie</td><td align="right">3,353</td><td align="right">$13,400.00</td></tr>
    <tr><td>Cake</td><td align="right">3,467</td><td align="right">$10,427.00</td></tr>
    <tr><td>Coffee</td><td align="right">3,551</td><td align="right">$7,158.00</td></tr>
    <tr><td>Tea</td><td align="right">3,319</td><td align="right">$5,015.50</td></tr>
    <tr><td>Cookie</td><td align="right">3,249</td><td align="right">$3,303.00</td></tr>
  </tbody>
</table>

<p>
<strong>Key Observation:</strong> Juice generated the highest recorded revenue among the products.
</p>

<h3>2. Payment Method Analysis</h3>

<table>
  <thead>
    <tr>
      <th>Payment Method</th>
      <th>Revenue</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Digital Wallet</td><td align="right">$48,526.50</td></tr>
    <tr><td>Credit Card</td><td align="right">$20,539.00</td></tr>
    <tr><td>Cash</td><td align="right">$20,526.50</td></tr>
  </tbody>
</table>

<p>
<strong>Key Observation:</strong> Digital Wallet was the dominant payment method, indicating strong customer adoption of digital payments.
</p>

<h3>3. Location Analysis</h3>

<table>
  <thead>
    <tr>
      <th>Location</th>
      <th>Revenue</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Takeaway</td><td align="right">$62,241.00</td></tr>
    <tr><td>In-store</td><td align="right">$27,351.00</td></tr>
  </tbody>
</table>

<p>
<strong>Key Observation:</strong> Takeaway transactions generated the majority of the recorded revenue.
</p>

<h3>4. Monthly Revenue Trend</h3>

<table>
  <thead>
    <tr>
      <th>Month</th>
      <th>Revenue</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>January</td><td align="right">$7,306.00</td></tr>
    <tr><td>February</td><td align="right">$6,681.50</td></tr>
    <tr><td>March</td><td align="right">$7,246.50</td></tr>
    <tr><td>April</td><td align="right">$7,248.00</td></tr>
    <tr><td>May</td><td align="right">$7,037.50</td></tr>
    <tr><td>June</td><td align="right">$7,382.00</td></tr>
    <tr><td>July</td><td align="right">$11,091.00</td></tr>
    <tr><td>August</td><td align="right">$7,125.50</td></tr>
    <tr><td>September</td><td align="right">$6,910.00</td></tr>
    <tr><td>October</td><td align="right">$7,334.00</td></tr>
    <tr><td>November</td><td align="right">$6,989.00</td></tr>
    <tr><td>December</td><td align="right">$7,241.00</td></tr>
  </tbody>
</table>

<p>
<strong>Key Observation:</strong> July recorded the highest monthly revenue, while February recorded the lowest.
</p>

<h2>📐 Statistical Analysis</h2>

<p>
The following statistics were calculated using the <strong>Total Spent</strong> column.
</p>

<table>
  <thead>
    <tr>
      <th>Statistical Metric</th>
      <th>Value</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Total Transactions</td><td align="right"><strong>10,000</strong></td></tr>
    <tr><td>Total Revenue / Total Spent</td><td align="right"><strong>$89,592.00</strong></td></tr>
    <tr><td>Average Transaction</td><td align="right">$8.9592</td></tr>
    <tr><td>Minimum Transaction</td><td align="right">$1.00</td></tr>
    <tr><td>Maximum Transaction</td><td align="right">$25.00</td></tr>
    <tr><td>Total Quantity Sold</td><td align="right">30,271</td></tr>
    <tr><td>Average Quantity</td><td align="right">3.0271</td></tr>
    <tr><td>Median Transaction</td><td align="right">$8.00</td></tr>
    <tr><td>Transaction Std. Dev.</td><td align="right">6.0090</td></tr>
    <tr><td>Q1</td><td align="right">$4.00</td></tr>
    <tr><td>Q3</td><td align="right">$12.00</td></tr>
    <tr><td>IQR</td><td align="right">$8.00</td></tr>
    <tr><td>Lower Bound</td><td align="right">-$8.00</td></tr>
    <tr><td>Upper Bound</td><td align="right">$24.00</td></tr>
    <tr><td>Potential Outliers</td><td align="right"><strong>268</strong></td></tr>
  </tbody>
</table>

<h2>🚨 Outlier Analysis</h2>

<p>
The <strong>Interquartile Range (IQR)</strong> method was used to identify potential high-value transactions.
</p>

<ul>
  <li>Q1 = $4</li>
  <li>Q3 = $12</li>
  <li>IQR = $8</li>
  <li>Lower Bound = -$8</li>
  <li>Upper Bound = $24</li>
</ul>

<p>
Transactions above <strong>$24</strong> were considered potential high-value outliers.
</p>

<p>
<strong>Result:</strong> 268 transactions have a <code>Total Spent</code> value of <strong>$25.00</strong>.
</p>

<h2>📊 Charts and Visualizations</h2>

<ul>
  <li>Revenue by Item</li>
  <li>Quantity Sold by Item</li>
  <li>Monthly Revenue Trend</li>
  <li>Revenue by Payment Method</li>
  <li>Revenue by Location</li>
</ul>

<h2>💡 Key Insights</h2>

<h3>1. Product Performance & Beverage Demand</h3>

<p>
Juice was the strongest-performing product, generating <strong>$19,128.50</strong>
in recorded Total Spent from <strong>6,435 units sold</strong>.
This indicates strong customer demand for the product.
</p>

<h3>2. Digital Payment Adoption</h3>

<p>
Digital Wallet generated <strong>$48,526.50</strong>, making it the leading payment method
by recorded transaction value. This indicates strong customer preference for convenient digital payment options.
</p>

<h3>3. Off-Premise Sales Performance</h3>

<p>
Takeaway transactions generated <strong>$62,241.00</strong>, significantly higher than in-store sales.
This highlights the importance of convenience and off-premise purchasing in overall sales performance.
</p>

<h3>4. Monthly Revenue Trend</h3>

<p>
<strong>July</strong> recorded the highest monthly revenue at <strong>$11,091.00</strong>,
while <strong>February</strong> recorded the lowest at <strong>$6,681.50</strong>.
This variation can help in seasonal planning, inventory management, and promotional strategies.
</p>

<h3>5. Customer Spending Behavior</h3>

<p>
The average transaction value was approximately <strong>$8.96</strong>, compared with a median of
<strong>$8.00</strong>. The higher average indicates that some higher-value transactions are increasing
the overall average spending.
</p>

<h3>6. High-Value Transaction Anomalies</h3>

<p>
Using the IQR method, the upper transaction-value threshold was <strong>$24.00</strong>.
The analysis identified <strong>268 transactions at $25.00</strong> as potential high-value outliers requiring further review.
</p>

<h3>7. Product Mix & Pricing Impact</h3>

<p>
Products with similar quantities sold can generate significantly different revenue because of differences
in price and recorded transaction value.
</p>

<h2>🔄 EDA Workflow</h2>

<pre>
Cleaned Dataset
       ↓
Data Exploration
       ↓
Pivot Tables
       ↓
Statistical Analysis
       ↓
Trend & Pattern Identification
       ↓
Outlier Detection
       ↓
Pivot Charts
       ↓
Business Insights
</pre>

<h2>📚 Learning Outcomes</h2>

<ul>
  <li>Perform Exploratory Data Analysis using Microsoft Excel.</li>
  <li>Work with cleaned datasets.</li>
  <li>Use Excel formulas for statistical analysis.</li>
  <li>Create and interpret Pivot Tables.</li>
  <li>Build Pivot Charts for data visualization.</li>
  <li>Analyze trends and patterns.</li>
  <li>Apply the IQR method for outlier detection.</li>
  <li>Identify anomalies in transaction data.</li>
  <li>Convert data findings into meaningful business insights.</li>
</ul>

<h2>📌 Key Results</h2>

<table>
  <tbody>
    <tr><td><strong>Total Transactions</strong></td><td>10,000</td></tr>
    <tr><td><strong>Total Units Sold</strong></td><td>30,271</td></tr>
    <tr><td><strong>Total Recorded Transaction Value</strong></td><td>$89,592.00</td></tr>
    <tr><td><strong>Average Transaction</strong></td><td>$8.96</td></tr>
    <tr><td><strong>Top Product</strong></td><td>Juice</td></tr>
    <tr><td><strong>Top Payment Method</strong></td><td>Digital Wallet</td></tr>
    <tr><td><strong>Top Location</strong></td><td>Takeaway</td></tr>
    <tr><td><strong>Highest Revenue Month</strong></td><td>July</td></tr>
    <tr><td><strong>Potential Outliers</strong></td><td>268</td></tr>
  </tbody>
</table>

<h2>📂 Project File</h2>

<p>
<strong>Excel Workbook:</strong> <code>cafe_sales_cleaned.xlsx</code>
</p>
<h2>📸 EDA Analysis Screenshots</h2>

<p>
The following screenshots show the Excel-based Exploratory Data Analysis,
statistical calculations, visualizations, and final insights developed for this project.
</p>

<h3>📊 EDA Analysis – Part 1</h3>

<p align="center">
  <img src="SWYNEX EDA Analysis1.png" alt="SWYNEX EDA Analysis 1" width="900">
</p>

<h3>📊 EDA Analysis – Part 2</h3>

<p align="center">
  <img src="SWYNEX EDA Analysis2.png" alt="SWYNEX EDA Analysis 2" width="900">
</p>

<h3>📊 EDA Analysis – Part 3</h3>

<p align="center">
  <img src="SWYNEX EDA Analysis3.png" alt="SWYNEX EDA Analysis 3" width="900">
</p>

<h3>📐 Statistical Calculations</h3>

<p align="center">
  <img src="SWYNEX EDA Calculations.png" alt="SWYNEX EDA Calculations" width="900">
</p>

<h3>💡 Final Insights</h3>

<p align="center">
  <img src="SWYNEX EDA Insights.png" alt="SWYNEX EDA Insights" width="900">
</p>
<h2>🏁 Conclusion</h2>

<p>
This Exploratory Data Analysis provides a clear view of product performance, customer spending,
payment preferences, sales locations, monthly trends, and potential anomalies in the cafe sales dataset.
</p>

<p>
The analysis demonstrates how Microsoft Excel-based EDA can transform raw transaction data into useful
business insights that can support sales planning, customer engagement, payment strategy,
inventory planning, and operational decision-making.
</p>

<hr>

<p align="center">
  <strong>SWYNEX Internship – Task 2 | Exploratory Data Analysis</strong>
</p>
