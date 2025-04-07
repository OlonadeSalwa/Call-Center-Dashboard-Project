# Call-Center-Dashboard-Project
This project analyzes 32,941 inbound calls from a call center dataset using Microsoft Excel to uncover customer interaction trends

## Dataset Used
- **Call Center Dataset**

## Dataset Source
  **Dataset was from kaggle**

## Tools Used
- **Microsoft Excel**

---
## Data Analysis Process

### 1. Data Preparation
- Opened the dataset in Excel and created a copy of the original data sheet:
  - Clicked on the sheet tab at the bottom, selected *Move or Copy*, chose *Move to End*, and checked *Create a copy*.
  - Renamed the copied sheet as `Working Sheet` for modifications.
- Adjusted the column width for better readability by selecting all columns and double-clicking the column separators.
- Differentiated the header row from the dataset:
  - Selected the header row, applied *Cell Style* from the *Home* tab, and bolded the text.
- Freezing the header row for easier scrolling:
  - Went to the *View* tab → Selected *Freeze Panes* → Clicked *Freeze Top Row*.
- Checked the number of records:
  - Selected a unique identifier (ID column), pressed `Ctrl + End`, and verified that the dataset contains **32,941 rows**.
  - Ensured there were no blank rows in the dataset by checking if navigation went to the last row seamlessly.
  - Used `Ctrl + Home` to return to the top of the dataset.

---
### 2. Data Formatting and Cleaning
- Standardized data types for consistency:
  - **CSAT Score Column:** Changed format from *General* to *Number* and removed extra decimal places.
  - **Call Duration (Minutes) Column:** Changed format from *General* to *Number* and removed extra decimal places.
  - **Call Timestamp Column:** Converted mixed data types using *Text to Columns*:
    - Selected column → *Data* tab → *Text to Columns* → Chose *Delimited* → Selected *Date (MDY)* → Clicked *Finish*.
  - Added a new `Call Day` column:
    - Inserted a new column beside `Call Timestamp` and named it `Call Day`.
    - Used the formula: `=DAY(E2)` to extract the day from the timestamp.
    - Removed decimal places and applied auto-fill.
- Checked for duplicate values in the dataset:
  - Selected the `ID Column` → *Data* tab → *Remove Duplicates* → No duplicates were found.

---
### 3. Creating the Dashboard
- Created a new sheet named `Pivot_Table` for analysis.
- Built pivot tables for key insights:
  - **Calls by Sentiment** – Categorized interactions into *Positive, Neutral, Negative, and Very Negative*.
  - **Call Volume by Location** – Identified cities with the highest call volume.
  - **Call Categories by Inquiry Type** – Analyzed call distribution across billing, technical support, and general inquiries.
  - **Response Time Analysis** – Compared resolved calls within and outside SLA limits.
- Designed an interactive dashboard incorporating:
  - Bar charts, pie charts, and slicers for sentiment and location-based analysis.
  - KPIs showing total calls, average CSAT score, and response time trends.

View my dashboard [Here](call_center_dashoard)

---
## Conclusion & Recommendations

### Key Findings
- **Call Volume Analysis:** The dataset recorded **32,941 inbound calls**, confirming that traditional call centers still handle high volumes despite the rise of digital channels like chatbots and email support.
- **Sentiment Analysis:** While many calls had a *neutral* sentiment, a significant portion had *negative* and *very negative* sentiments, highlighting areas for service improvement.
- **Regional Insights:** Los Angeles and Baltimore had the highest call volumes, indicating higher customer demand in these locations.
- **Inquiry Type:** Billing inquiries accounted for the majority of customer concerns, emphasizing the need for clear and transparent financial communication.
- **Response Time:** Most calls were resolved within SLA limits, but a fraction exceeded expected response windows, potentially affecting customer satisfaction.

### Actionable Recommendations
- **Improve Customer Service Training:** Focus on handling negative interactions and reducing response time in key locations like Los Angeles and Baltimore.
- **Enhance Self-Service Options:** Optimize chatbot efficiency to reduce call volumes related to billing inquiries.
- **Streamline Billing Communication:** Simplify financial communication and documentation to minimize confusion and reduce billing-related calls.
- **Optimize Staffing Strategy:** Allocate more resources to high-demand locations and peak hours to improve service delivery.

By leveraging these insights, businesses can enhance customer experience, optimize operations, and drive higher customer satisfaction.

See documentation [Here](https://docs.google.com/spreadsheets/d/1a3jm2Am52Lfs4BRLpocIRlbc6hvzXtGz/edit?usp=drive_link&ouid=107598010287273134190&rtpof=true&sd=true)
