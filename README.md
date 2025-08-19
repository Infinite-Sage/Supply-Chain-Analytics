# Supply Chain Analytics: Make vs. Buy Decision Support  

## 📌 Overview  
This project builds a **dynamic decision-support tool in Power BI** to guide supply chain teams through one of the most critical questions:  
👉 *Should we manufacture a part in-house (Make) or purchase it from an external supplier (Buy)?*  

The project was developed as part of a case study and demonstrates how **data modeling, DAX calculations, and interactive visuals** can provide clarity, consistency, and real-time flexibility for supply chain strategy.  

---

## 🎯 Objectives  
- Develop a **baseline data model** for supply chain cost analysis.  
- Calculate **extended cost** and **full cost** for supplier quotes.  
- Incorporate **scenario analysis** to test costs under varying production volumes.  
- Add **internal manufacturing costs** (capacity, overhead, capital investments).  
- Build a **Make vs. Buy model** comparing both options dynamically.  
- Integrate **quality/yield rates** to reflect real-world supplier performance.  
- Deliver an **interactive Power BI dashboard** for supply chain decision-making.  

---

## 🛠️ Methodology  

### 1. Data Modeling  
- Imported supplier quote data, internal cost estimates, and product dimensions.  
- Built relationships between supplier, part numbers, and cost factors.  
- Structured tables for **Scenario Volumes** and **Yield Rates**.  

### 2. Key Calculations (DAX)  
- **Extended Cost** = Unit Cost × Volume.  
- **Full Cost** = Extended Cost + Non-Recurring Expenses.  
- **Scenario Analysis** = Dynamic cost calculations across volume ranges.  
- **Make Scenario Cost** = Internal manufacturing full cost with capital requirements.  
- **Make vs. Buy Measure** = Logic to determine the cheaper option at a given volume.  
- **Cost Avoidance** = Savings from choosing the lower-cost option.  
- **Yield-Adjusted Costs** = Adjusted supplier cost considering defect/rework rates.  

### 3. Visualizations  
- **Make vs. Buy table** by part and supplier.  
- **Clustered column charts** showing supplier cost breakdowns.  
- **Scenario slicers** allowing interactive what-if analysis for volumes.  
- **Cost avoidance visuals** to quantify decision impact.  

---

## 📊 Key Findings  
- **Dynamic thresholds:** Some parts were cheaper to buy at low volumes but more economical to make internally at higher volumes.  
- **Supplier quality matters:** Yield rate adjustments shifted supplier rankings, proving cost alone is insufficient.  
- **Scalability:** The Power BI model adapts instantly when new quotes, parts, or volumes are added.  
- **Decision speed:** What-if sliders enabled leadership to adjust assumptions *live in meetings* instead of waiting for manual recalculations.  

---

## 🚀 Why Power BI (vs. Spreadsheets)?  
- **Consistency:** One data model, reusable across projects.  
- **Control:** Raw data integrity is preserved—reduces errors vs. spreadsheets.  
- **Real-time analysis:** Interactive slicers replace static models.  
- **Scalable sharing:** Dashboards can be securely shared across teams.  

---

## 📂 Repository Contents  
- `Supply Chain Analytics.pbix` → Full Power BI solution file.  
- `README.md` → Project documentation.
- `Fictitious RFP Responses for Make vs Buy.xlsx` → dataset
- (Optional future: add raw data CSVs or mock datasets for replication.)  

---

## 🔮 Future Work  
This project is a **baseline model** that can be extended with:  
- Freight, logistics, and **lead time costs**.  
- **Multi-facility production** and resource constraints.  
- **Variable overhead rates** and salaried labor.  
- **Risk analysis** (supply chain disruptions, geopolitical risks).  
- **Automation** with Power BI Service + scheduled refresh from ERP/CRM systems.  

---

## 🧑‍💻 How to Use / Replicate  
1. Download the `.pbix` file.  
2. Open in **Power BI Desktop**.  
3. Review data model (`Model view`).  
4. Explore and adjust the DAX measures in `Scenario Volume` and `Quotes` tables.  
5. Use slicers (e.g., Scenario Volume) to replicate the dynamic analysis.  

*Note: For confidentiality, sample/mocked data may be used in this version. Replace with your own supplier/manufacturing data for real-world deployment.*  

---

## 📢 Acknowledgments  
This project was inspired by supply chain analytics coursework and hands-on Power BI case studies. 

---

