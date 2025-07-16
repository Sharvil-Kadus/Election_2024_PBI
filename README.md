# Election_2024_PBI
Election_2024_PBI_Dashboard



# 🗳️ India General Election Result Dashboard – 2024  
**📅 Dataset**: Indian General Elections 2024  
**🔧 Tool Used**: Power BI Desktop

## 📌 Overview  
This dashboard visualizes the results of the 2024 Indian General Elections, offering a comprehensive view of alliance-wise seat distribution, party performance by state, and constituency-level details. It serves as a geo-political analysis tool to explore voting outcomes and trends across India’s diverse electoral map.

---

## ⚙️ Technical Design  

- **Modeling Architecture**:  
  - Fact table with constituency-level voting details  
  - Dimension tables for State, Party, Alliance, Candidate metadata  
  - Integrated geospatial layers for state-wise and district-wise mapping

- **Power Query Transformations**:  
  - Cleaned up location mismatches, normalized party abbreviations  
  - Split vote columns into EVM and postal ballots  
  - Calculated margins and vote shares dynamically

- **DAX Calculations**:
  ```DAX
  Total Votes = [EVM Votes] + [Postal Votes]  
  Vote Share % = DIVIDE([Total Votes], [Constituency Total Votes])  
  Margin = [Winning Votes] - [Runner-Up Votes]
  ```

- **Visual Elements**:  
  - Map visuals highlighting alliance dominance state-wise  
  - Stacked column charts for seat count by party and alliance  
  - Tables and tooltips for constituency-level candidate comparison  
  - State drill-through for localized breakdowns  

---

## 🔢 Key Statistics  

| Metric                         | Value        |
|--------------------------------|--------------|
| Total Seats                    | 543          |
| NDA Alliance Seats             | 292 (54%)    |
| INDIA Alliance Seats           | 234 (43%)    |
| Other/Independent Seats        | 17 (3%)      |
| Participating NDA Parties      | 14           |
| Participating INDIA Parties    | 20           |
| Maharashtra Total Seats        | 48           |
| Leading State (NDA)            | Maharashtra (30 seats) |

---

## 🗂 Constituency Analysis  

- **Ahmednagar (Maharashtra)**:  
  - Winner: Nilesh Dnyandev Lanke (NCPSP – INDIA)  
  - Vote Share: 47.14%  
  - Runner-up: Dr. Sujay Vikhe Patil (NCPSP – INDIA)  
  - Margin: 28,929 votes  

- **Other Key Examples**:  
  - BJP dominance in Gujarat constituencies like Ahmedabad West and Agra  
  - Close contests in Kerala and UP between INC and BJP candidates  
  - Independent candidates visible in select constituencies with small vote shares

---

## 🧭 Use Case Focus  

- **Political Research**: Breakdown of alliance strength across regions  
- **Journalistic Reporting**: Visual summaries and comparative results  
- **Civic Awareness**: Constituency-level transparency for voters  
- **Geopolitical Strategy**: Analyzing swing regions and voter behavior patterns

---

## 💼 Project Value  
This dashboard reflects expertise in:
- Handling large structured political datasets  
- Mapping party alliances to voting patterns via BI tools  
- Geospatial visuals layered with dynamic DAX metrics  
- Clean and scalable design fit for public sector analytics, civic data transparency, and portfolio presentation



