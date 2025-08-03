# 🏆 [Power BI Dataviz World Champs | EU Edition](https://aka.ms/WorldChampsEU)

## Europe by the Numbers - World Champs Data and Starter File

This repository contains the dataset and Power BI starter file for the **Power BI Dataviz World Champs** contest, EU edition. 

The Power BI starter file helps you explore quality of life, culture, and sustainability across Europe over time, using four standardized indicators linked by country and year. You are welcome to use the starter file, but not required. What is required is that you include data in your submission from at least one of the included fact tables. You also must stick to the theme, looking at quality of life in Europe over time. Feel free to add supplemental data!

🔗 **Contest announcement & instructions:**  👉 [Power BI DataViz World Championships](https://aka.ms/WorldChampsEU)

---

## 📁 What's Included

- `World Champs EU Starter File.pbix` — Power BI file with ready-to-use semantic model and table visual
- `README.md` — This documentation
- No data files are included in this repository — see below for download instructions

---

## 🔽 How to Download the Starter File

If you're not familiar with GitHub, here’s how to download the Power BI file:

Navigate to the folder:

1. FabricCommunityContest/StarterFiles

1. Click on the .pbix file.

1. Click the Download button (or right-click and choose Save link as...).

You don’t need to clone the repository — just download the file directly.

---

## 🔽 How to Download the Data

If you are using the starter file, you'll want to download the source data (with the exception of the Country Code Mapping) if you want to make any changes to the data in Power Query, including the addition of supplemental data. **You do not have to download the data** if you do not plan to make any changes to the starter semantic model. 

To keep this repository clean and aligned with data licensing terms, **no data files are stored here**. Instead, follow the links below to download the source CSVs directly from trusted public data providers:

### 📊 Source Data

1. **Renewable energy share (% of gross final energy consumption)** <br>
      [Eurostat](https://db.nomics.world/Eurostat/nrg_ind_ren)

1. **Life satisfaction data: Overall life satisfaction by sex, age and educational attainment** <br>
      [Eurostat](https://ec.europa.eu/eurostat/databrowser/bookmark/74e5d311-1b68-4b8b-9269-15f35206d404)

1. **Participation in cultural activities: Persons participating in cultural or sport activities in the last 12 months by sex, age, educational attainment, activity type and frequency** <br>
      [Eurostat](https://ec.europa.eu/eurostat/databrowser/view/ilc_scp03/default/table)

1. **Country flags** <br>
      [Flagpedia.net/Wikipedia Commons SVGs](https://flagcdn.com)

1. **Population by Country and Year**  <br>
      [Our World in Data](https://ourworldindata.org/grapher/population)

1. **Country Code Mapping (ISO3 → ISO2)**  
      [GitHub](https://raw.githubusercontent.com/lukes/ISO-3166-Countries-with-Regional-Codes/refs/heads/master/all/all.csv)

If you have questions about the source data, please add a comment to the [Dataviz World Champs contest page](https://aka.ms/WorldChampsEU).

📁 If you plan to use the starter file, we've created a parameter in the file for you (for ease of use). Once downloaded, place all data files in the same local folder. Then follow the steps below to connect them to the Power BI file. You do **not** have to use the starter file, it's provided to help you but is not a requirement.

💡 Reminder - it is required that you use data from one of the first 3 files listed here: **Renewable energy share**, **life satisfaction data**, or **participation in cultural activities**.

---

## ⚙️ How to Use the Starter File

1. Open the `World Champs EU Starter` file in Power BI Desktop.
2. Go to **Home > Transform Data > Edit Parameters**
3. Paste the full path to the folder where you saved the source csv and XLSX files.  
   👉 Example: C:\Users\YourName\Downloads\Data
4. Click **OK**, then **Close & Apply** to load the data.

---

## 🧠 Semantic Model Overview

This report brings together five open data sources to explore well-being, culture, sustainability, and demographics across European countries. The model is structured using a star schema with two dimension tables and four fact tables:

### Dimension Tables

- **Countries**: Contains country names, ISO codes (alpha-2 and alpha-3), flags, and region/sub-region classifications.

- **Years**: A simple list of years from 2000 to 2025, used to align time series data.

### Fact Tables

- **Population**: Total national population per year. Useful for normalization (e.g., per capita metrics).

- **Life Satisfaction**: Average life satisfaction score (0–10) by country and year.

- **Cultural Activity Participation**: % of population that attended cultural events (e.g., concerts, museums) per year.

- **Renewable Energy**: Share of energy from renewable sources (%) by country and year.

All fact tables link to the Countries and Years dimensions using one-to-many relationships, ensuring consistency and flexibility when analyzing trends over time or across regions.

---

## 🧑‍💻 License

This repository is provided under the MIT License. All third-party data remains under its original license or usage terms.

---

🎉 Happy visualizing — and good luck in the contest - we can't wait to see what you create!
