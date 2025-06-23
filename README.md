# 📊 Power BI 10th Birthday DataViz Contest: Tech Adoption Dataset

This repository contains the dataset and Power BI starter file for the **PBI10 Dataviz Contest**, created to celebrate Power BI’s 10th birthday! 🥳  
Participants can explore and visualize how technology adoption has changed globally over the past decade using standardized, per-100-person metrics.

🔗 **Contest announcement & instructions:**  
👉 [PBI10 Dataviz Contest](https://community.fabric.microsoft.com/t5/Power-BI-Community-Blog/Coming-soon-PBI10-Dataviz-Contest/ba-p/4738013)

---

## 📁 What's Included

- `PBI10_TechAdoption.pbix` — Power BI file with clean data model and visuals
- `data/` — Folder with all source data
  - `mobile-cellular-subscriptions-per-100-people.csv`
  - `fixed-telephone-subscriptions-per-100-people.csv`
  - `share-of-individuals-using-the-internet.csv`
  - `population.csv`
  - `country-code-mapping.csv` (ISO3 to ISO2 for flag images)

---

## 🧠 Data Model

The Power BI file uses 3 key tables:

| Table      | Description                                      |
|------------|--------------------------------------------------|
| `Countries`| Country metadata (name, ISO codes, region, income group) |
| `Years`    | Calendar years used to explore trends over time |
| `Data`     | Contains per-100-person values for each metric:  
             `LandlineUsersPer100`, `MobileUsersPer100`, `InternetUsersPer100`

---

## ⚙️ How to Use the File

1. Open the `PBI10_TechAdoption.pbix` file in Power BI Desktop.
2. If prompted to update the folder path:
   - Go to **Home > Transform Data > Edit Parameters**
   - Enter the full path to your local `data/` folder.
   - Click **OK**, then **Close & Apply**
3. Explore the data with the provided visuals or build your own!

---

## 🌍 Data Sources & Citation

All data is sourced from **Our World in Data** and processed using open-source datasets originally published by the **International Telecommunication Union (ITU)** and the **World Bank**.

### 📚 Full Citation

> International Telecommunication Union (ITU) via World Bank, UN World Population Prospects, and Gapminder — processed by Our World in Data.  
> Mobile cellular subscriptions (per 100 people); Fixed telephone subscriptions (per 100 people); Share of individuals using the internet; and Population by country and year.  
> Retrieved from Our World in Data:  
> - https://ourworldindata.org/grapher/mobile-cellular-subscriptions-per-100-people  
> - https://ourworldindata.org/grapher/fixed-telephone-subscriptions-per-100-people  
> - https://ourworldindata.org/grapher/share-of-individuals-using-the-internet  
> - https://ourworldindata.org/grapher/population

All charts and data from Our World in Data are made available under the **Creative Commons BY license**. Please cite appropriately when using or sharing.

Learn more about data reuse: https://ourworldindata.org/about#how-do-i-cite-your-work

---

## 🖼️ Attribution Note

Flag image URLs are constructed using ISO2 country codes from [flagcdn.com](https://flagcdn.com), a free and open CDN of SVG/PNG flags.

---

## 🧑‍💻 License

This repository is provided for educational and contest purposes under the MIT License. All third-party data remains under its original license.

---

🎉 Happy visualizing — and good luck in the #PBI10 contest!
