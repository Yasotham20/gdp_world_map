# gdp_world_map
Here’s a complete and detailed `README.md` for your GDP World Map Plotter project, Dharani. It includes project overview, setup instructions, usage examples, sample output, technologies used, and helpful links.

---

```markdown
# 🌍 GDP World Map Plotter

This project visualizes global GDP data on an interactive world map using Python and Pygal. It processes World Bank GDP data from a CSV file, reconciles country names between Pygal and the dataset, and plots the logarithm (base 10) of GDP values for a selected year. The output is an SVG map that highlights countries with GDP data, countries missing from the dataset, and countries with no data for the selected year.

---

## 📦 Project Structure

```
gdp_world_map/
├── gdp.csv                      # GDP data file (World Bank format)
├── gdp_plotter.py              # Main Python script
├── isp_gdp_world_name_2000.svg # Sample output map
└── README.md                   # Project documentation
```

---

## 🚀 Features

- Reads and cleans GDP data from a structured CSV file
- Matches country names between Pygal codes and World Bank entries
- Applies log scaling to GDP values for better color distribution
- Generates SVG maps for any year between 1960 and 2015
- Highlights countries with missing or incomplete data

---

## 🧰 Technologies Used

- Python 3.x
- Pygal (for SVG map rendering)
- CSV module (for file parsing)
- Math module (for log scaling)

---

## 📥 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/gdp-world-map.git
   cd gdp-world-map
   ```

2. Install dependencies:
   ```bash
   pip install pygal
   ```

3. Make sure `gdp.csv` is in the project folder.

---

## 🧪 Usage

Run the script in Python:

```python
from gdp_plotter import render_world_map, build_map_dict_by_name
from pygal.maps.world import COUNTRIES

gdpinfo = {
    "gdpfile": "gdp.csv",
    "separator": ",",
    "quote": '"',
    "min_year": "1960",
    "max_year": "2015",
    "country_name": "Country Name",
    "country_code": "Country Code"
}

render_world_map(gdpinfo, COUNTRIES, "2000", "isp_gdp_world_name_2000.svg")
```

To preview the map in your browser:
```python
worldmap.render_in_browser()
```

---

## 📊 Sample Output

![Sample GDP Map](https://raw.githubusercontent.com/your-username/gdp-world-map/main/isp_gdp_world_name_2000.svg)

---

## 📚 References

- [World Bank GDP Data](https://data.worldbank.org/indicator/NY.GDP.MKTP.CD)
- [Pygal Documentation](http://www.pygal.org/en/latest/documentation/types/maps/worldmap.html)
- [Python CSV Module](https://docs.python.org/3/library/csv.html)
- [Math Logarithm Function](https://docs.python.org/3/library/math.html#math.log10)

---

## 🧠 Project Goals

- Practice working with dictionaries and CSV files
- Learn to reconcile multiple datasets
- Explore data visualization with Pygal
- Build a clean, reusable data pipeline

---

## 📝 License

This project is for educational use. You are free to modify and share it with proper attribution.

---

## 🙋‍♀️ Author

**Yasotha M** – Final-year BE. Computer Science and Engineering student at Apollo Engineering College, Chennai.

---

```

Let me know if you want this saved as a file or customized with your GitHub username and repo link!
