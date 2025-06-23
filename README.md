# 📊 Power BI 10th Birthday DataViz Contest: Tech Adoption Dataset

This repository contains the dataset and Power BI starter file for the **PBI10 Dataviz Contest**, created to celebrate Power BI’s 10th birthday! 🥳  

Participants can explore and visualize how technology adoption has changed globally over the past decade using standardized, per-100-person metrics.

🔗 **Contest announcement & instructions:**  👉 [PBI10 Dataviz Contest](https://community.fabric.microsoft.com/t5/Power-BI-Community-Blog/Coming-soon-PBI10-Dataviz-Contest/ba-p/4738013)

---

## 📁 What's Included

- `PBI10 Starter File.pbix` — Power BI file with clean data model and visuals
- `README.md` — This documentation
- No data files are included in this repository — see below for download instructions

---

## 🔽 How to Download the Data

To keep this repository clean and aligned with data licensing terms, **no data files are stored here**. Instead, follow the links below to download the source CSVs directly from trusted public data providers:

### 📊 Required Datasets (CSV format)

1. **Mobile Cellular Subscriptions**  
   https://ourworldindata.org/grapher/mobile-cellular-subscriptions-per-100-people

2. **Fixed Telephone (Landline) Subscriptions**  
   https://ourworldindata.org/grapher/fixed-telephone-subscriptions-per-100-people

3. **Internet Users (% of Population)**  
   https://ourworldindata.org/grapher/share-of-individuals-using-the-internet

4. **Population by Country and Year**  
   https://ourworldindata.org/grapher/population

5. **Country Code Mapping (ISO3 → ISO2)**  
   https://raw.githubusercontent.com/lukes/ISO-3166-Countries-with-Regional-Codes/refs/heads/master/all/all.csv

📁 Once downloaded, place all CSVs in the same local folder. Then follow the steps below to connect them to the Power BI file.

---

## ⚙️ How to Use the File

1. Open the `PBI10 Starter` file in Power BI Desktop.
2. Go to **Home > Transform Data > Edit Parameters**
3. Paste the full path to the folder where you saved the CSV files.  
   👉 Example: C:\Users\YourName\Downloads\PBI10Data
4. Click **OK**, then **Close & Apply** to load the data.

---

## 🧠 Data Model Overview

| Table      | Description                                      |
|------------|--------------------------------------------------|
| `Countries`| Country name, ISO codes, region, income group, flag URL |
| `Years`    | Calendar years for analysis                     |
| `Data`     | Per-100-person metrics by country and year: `LandlineUsersPer100`, `MobileUsersPer100`, `InternetUsersPer100` |

All values are standardized and ready for comparison across time and geography.

---

## 📚 Citation

> International Telecommunication Union (ITU) via World Bank, UN World Population Prospects, Gapminder — processed by Our World in Data.  
> *Mobile cellular subscriptions (per 100 people); Fixed telephone subscriptions (per 100 people); Share of individuals using the internet; and Population by country and year.*  
> Retrieved from Our World in Data:  
> - https://ourworldindata.org/grapher/mobile-cellular-subscriptions-per-100-people  
> - https://ourworldindata.org/grapher/fixed-telephone-subscriptions-per-100-people  
> - https://ourworldindata.org/grapher/share-of-individuals-using-the-internet  
> - https://ourworldindata.org/grapher/population

**Country code mapping dataset**:  
> GitHub user [@lukes](https://github.com/lukes) — [ISO 3166 Countries with Regional Codes (CSV)](https://github.com/lukes/ISO-3166-Countries-with-Regional-Codes)

Our World in Data content is available under the [Creative Commons BY license](https://ourworldindata.org/about#how-do-i-cite-your-work). Always provide attribution and cite third-party data providers as well.

---

## 🖼️ Flags

Flag image URLs are generated using 2-letter ISO codes and the free CDN at [flagcdn.com](https://flagcdn.com).  
Data model includes a column for these URLs in the `Countries` table — simply set the **Data Category** to `Image URL` in Power BI to display flags.

---

## 🧑‍💻 License

This repository is provided under the MIT License. All third-party data remains under its original license or usage terms.

---

🎉 Happy visualizing — and good luck in the #PBI10 contest!
