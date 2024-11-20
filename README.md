# Supplier Quality & Performance Analysis

### Executive Summary
Using Power BI, I created a comprehensive report to track supplier performance and reduce downtime. 
After identifying a direct correlation between downtime and financial losses, I recommend that manufacturers emphasise the financial impact of production delays beyond tracking defect quantities and downtime.
Interact with dashboard [here](https://app.powerbi.com/view?r=eyJrIjoiMDk4NmFjY2YtM2UzNy00MTFiLWJhNzAtYWYwYTc3YjMzMjIyIiwidCI6ImQzM2ZkNjEzLTdjZmItNDZhMC04MmZlLTI5NDg1ZDUwMDFkZSJ9&pageName=fa6f8390970637b60a6a).

### Problem Statement
Enterprise Manufacturers Ltd. had no procurement system put in place to validate supplier performance across different plants. 
The lack of visibility into supplier quality resulted in frequent downtime and inconsistent production outputs. 
As the management team aimed to centralize this information, the following key questions were raised:
1. Which vendors/plants are causing the greatest defect quantity?
2. Which vendors/plants are causing the greatest downtime?
3. Are there particular combinations of materials and vendors that perform poorly?
4. How does the same vendor and material perform across different plants?
5. Are there any insights or patterns the team may have overlooked?

The business needed a clear, data-driven approach to visualize and answer these questions.

### Methodology
Although the data required minimal cleaning, establishing an efficient data model was crucial to improving performance and optimizing the report generation process. 
The existing “one-table” data model is cumbersome, often resulting in longer-than-usual run times when generating reports. To address this, I focused on breaking out key dimensions into separate tables based on their attributes.

**Segmentation into Dimension Tables**: I created dimension tables with unique identifiers for categories like Vendor, Plant Location, Material Type, and Defect Type. 
The goal was to create a model that would allow for more efficient querying and insightful reporting. 

**Building the Fact Table**: Once the dimension tables were established, I used Power BI’s Merge Feature to integrate the keys back into the original dataset, forming a well-structured Fact Table.

**Creating a Date Table**: Using DAX (Data Analysis Expressions), I built an accurate Date Table that enabled effective time series analysis, making it easier to track trends over time.

**Star Schema Data Model**: I established relationships between tables by connecting the primary keys in the dimension tables to the foreign keys in the Fact Table. 
This resulted in a clean Star Schema Model. By organizing the data this way, you can be rest assured of generating reports without performance lags.

### Skills
- Data Modeling
- Power Query
- DAX
- Data Visualization
- Report design
  
### Key Insights Summary
**Rising Defects and Downtime**: Defect quantities surged to 2.6 billion units, with a corresponding increase in downtime to 216,000 hours, leading to a financial impact of $2.16 million underscoring the direct cost of defective materials on production efficiency.

**Financial Impact**: A crucial insight from the analysis is the direct correlation between downtime and financial losses. Assuming a downtime cost of $10 per hour, the company incurred over $2 million in downtime costs, with spikes in September and December indicating periods of severe disruption. This financial perspective provides stakeholders with a clear understanding of how supplier quality issues are affecting the bottom line.

**Worst-Performing Vendors**: Certain suppliers were identified as high-risk due to their consistent contribution to defects and downtime. Vendors like Avamm, Meejo, and Yombu emerged as the top offenders, contributing the highest defect quantities and significant downtime hours, reflecting the need for targeted supplier improvement initiatives.

**Plant-Specific Issues**: The analysis highlighted several plants, such as Hingham, Charles City, and Twin Rocks, as hotspots for defect-related downtime, with each plant reporting defect quantities nearing 100 million.

**Defect Categories**: Recurring issues like Bad Seams was the most frequent, requiring attention from both suppliers and internal quality control.

**Material Performance**: Raw materials were the most problematic, causing significant downtime. The rising trends in mechanical and logistics defects suggest a need for process and supply chain improvements.

**Vendor-Material/Plant Combinations**: The analysis drilled down into specific vendor-material and vendor-plant combinations to identify the worst performers. For example, the vendor Abata, when supplying raw materials, caused significant downtime and costs, with 3 million defects and 249 downtime hours, resulting in nearly $2,500 in lost productivity.

### Recommendations
1. **Centralize Data and Automate Reporting**: A centralized data management system is essential for tracking and evaluating supplier performance across multiple plants. Automating data collection and reporting will enhance visibility, reduce manual effort, and ensure consistency across operations.
2. **Focus on Financial Impact**: Beyond tracking defect quantities and downtime, manufacturers should emphasize the financial impact of production delays. This approach ensures that business leaders can directly see the cost implications of supplier quality issues, driving more urgent and informed decision-making.
3. **Implement a Continuous Improvement Program**: Based on the insights gathered from supplier performance data, manufacturers should establish a continuous improvement program focused on reducing downtime, improving material quality, and addressing recurring defects. This will drive supplier accountability and improve the overall efficiency of the supply chain.
4. **Leverage Advanced Analytics**: To further enhance supplier quality management, manufacturers can integrate advanced analytics and predictive models. By identifying patterns and trends early on, businesses can proactively address potential issues before they result in costly downtime or material waste.

### Conclusion
Business intelligence tools can revolutionize supplier quality management by transforming raw data into insightful, actionable reports. 
For Enterprise Manufacturers Ltd., the implementation of a BI-driven approach revealed trends, inefficiencies, and potential risks that would have otherwise gone unnoticed. 
By quantifying the financial impact of defective materials, the company was able to identify and address the root causes of production inefficiencies.
Centralizing procurement and performance data through Power BI will enable the management team to make more informed decisions regarding vendor performance, plant operations, and material selection. The analysis not only highlighted key performance gaps but has also paved the way for long-term process improvements.
