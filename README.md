# Battle of Cities: New York vs Toronto Neighborhood Analysis

**IBM Data Science Professional Certificate - Capstone Project**

**Author:** Oluwaseun Mesele  
**Course:** IBM Data Science Professional Certificate (Coursera)

---

## 📋 Project Overview

This project compares the similarities and differences between neighborhoods in **New York City** (Manhattan) and **Toronto** using data science techniques. The analysis uses **K-Means clustering** to group neighborhoods based on venue types, providing insights for business decisions such as optimal restaurant locations.

---

## 🎯 Business Problem

The goal is to answer:
1. How do neighborhoods in Manhattan (NYC) compare to neighborhoods in Toronto?
2. What are the most common venue types in each city's neighborhoods?
3. Where would be the best location to open a new restaurant in either city?

This analysis is valuable for:
- **Entrepreneurs** looking to open businesses in either city
- **Real estate investors** comparing neighborhood characteristics
- **Urban planners** understanding city similarities and differences

---

## 📊 Data Sources

| Data | Source | Description |
|------|--------|-------------|
| NYC Neighborhoods | IBM Coursera JSON file | Borough, neighborhood, latitude, longitude |
| Toronto Neighborhoods | Wikipedia + Geocoding | Postal codes, boroughs, neighborhoods, coordinates |
| Venue Data | Foursquare API | Venue names, categories, locations |

---

## 🛠️ Methodology

### 1. Data Collection
- Scraped Toronto neighborhood data from Wikipedia using **BeautifulSoup**
- Retrieved NYC neighborhood data from provided JSON file
- Obtained geospatial coordinates using geocoding APIs
- Fetched venue data using **Foursquare API**

### 2. Data Preprocessing
- Cleaned and formatted neighborhood data
- Filtered to focus on Manhattan (NYC) and Toronto-named boroughs
- One-hot encoded venue categories
- Grouped venues by neighborhood

### 3. Exploratory Data Analysis
- Analyzed most common venue types per neighborhood
- Visualized neighborhood distributions on **Folium maps**
- Compared venue category frequencies between cities

### 4. Machine Learning - K-Means Clustering
- Applied **K-Means clustering** to group similar neighborhoods
- Determined optimal number of clusters
- Analyzed cluster characteristics
- Compared clusters between NYC and Toronto

---

## 📁 Repository Structure

```
├── Battle_of_Cities.ipynb          # Main analysis notebook (START HERE)
├── Coursera_Capstone_IBM_datascience.ipynb  # Alternative analysis notebook
├── Finals_wk3_complete.ipynb       # Week 3 complete assignment
├── Finals_wk3_clustering.ipynb     # Clustering analysis
├── Finals_wk3_part1.ipynb          # Data collection
├── BeautifulSoup.ipynb             # Web scraping practice
├── intro_business_problem.ipynb    # Business problem statement
├── data_section.ipynb              # Data description
│
├── CAPSTONE_REPORT_COURSERA.pdf    # Final project report
├── IBM_DATA_SCIENCE.pdf            # Presentation slides (PDF)
├── IBM_DATA_SCIENCE.key            # Presentation slides (Keynote)
│
├── Data Files:
│   ├── manhattan_neighbourhoods.csv        # Manhattan neighborhood data
│   ├── torontonamed_beighborhoods.csv      # Toronto neighborhood data
│   ├── manhattan_grouped.csv               # Manhattan venues grouped
│   ├── toronto_grouped.csv                 # Toronto venues grouped
│   ├── manhattan_neighborhoods_sorted.csv  # Top venues per Manhattan neighborhood
│   ├── toronto_neighborhoods_sorted.csv    # Top venues per Toronto neighborhood
│   ├── NY_neighborhoods.csv                # Full NYC neighborhood data
│   ├── Toronto_Boroughs_LongLat.csv        # Toronto coordinates
│   ├── Geospatial_Coordinates.csv          # Additional coordinates
│   └── allnewyork_df.csv                   # Complete NYC dataset
│
└── README.md
```

---

## 🔧 Technologies Used

| Category | Tools |
|----------|-------|
| **Programming** | Python 3 |
| **Data Manipulation** | Pandas, NumPy |
| **Machine Learning** | Scikit-learn (K-Means Clustering) |
| **Visualization** | Matplotlib, Folium (Interactive Maps) |
| **Web Scraping** | BeautifulSoup, Requests |
| **APIs** | Foursquare Location API |
| **Geocoding** | Geopy |

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib folium beautifulsoup4 requests geopy
```

### Run the Analysis
1. Clone this repository
2. Open `Battle_of_Cities.ipynb` in Jupyter Notebook
3. Run all cells to reproduce the analysis

---

## 📈 Key Findings

### Venue Distribution
- **Manhattan**: High concentration of coffee shops, Italian restaurants, and bars
- **Toronto**: More diverse mix including cafés, coffee shops, and breakfast spots

### Clustering Results
- Both cities show distinct neighborhood clusters based on venue types
- Financial districts in both cities cluster together
- Residential areas show similar patterns across cities

### Business Recommendation
Based on the analysis, optimal locations for a new restaurant would be in neighborhoods with:
- Lower restaurant saturation
- High foot traffic (indicated by coffee shops, transit)
- Mixed residential/commercial character

---

## 📄 Reports & Presentations

- **[Full Report](CAPSTONE_REPORT_COURSERA.pdf)** - Detailed analysis and findings
- **[Presentation](IBM_DATA_SCIENCE.pdf)** - Summary slides

---

## 🎓 Certificate

This project was completed as part of the [IBM Data Science Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-science) on Coursera.

---

## 📬 Contact

**Oluwaseun Mesele**
- LinkedIn: [linkedin.com/in/oluwaseun-mesele](https://linkedin.com/in/oluwaseun-mesele)
- Email: seunmesele@gmail.com

---

## 📜 License

This project is for educational purposes as part of the IBM Data Science Professional Certificate program.
