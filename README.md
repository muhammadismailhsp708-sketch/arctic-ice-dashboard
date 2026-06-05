# 🧊 Arctic Sea Ice Extent Dashboard

**Course:** Exploratory Data Analysis  
**Instructor:** Ali Hassan Sherazi  
**Dataset:** `arctic_ice_extent.csv` *(exact file name retained as required)*

---

## 📌 Project Overview

An interactive Streamlit dashboard analyzing Arctic Sea Ice Extent from **1979 to 2023**.  
The dashboard visualizes trends, distributions, comparisons, and correlations using 10+ chart types with fully linked, dynamic filters.

---

## 🗂️ Project Structure

```
dashboard_project/
├── data/
│   └── arctic_ice_extent.csv       ← Original dataset (DO NOT rename)
├── notebooks/
│   └── analysis.ipynb              ← EDA notebook
├── app.py                          ← Main Streamlit dashboard
├── charts.py                       ← All chart/visualization functions
├── filters.py                      ← Data loading, cleaning, filter logic
├── requirements.txt                ← Python dependencies
└── README.md                       ← This file
```

---

## ⚙️ Installation & Setup

### 1. Clone / Download the project folder

### 2. Create a virtual environment (recommended)
```bash
python -m venv venv
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the dashboard
```bash
streamlit run app.py
```

The dashboard will open in your browser at `http://localhost:8501`

---

## 📊 Charts Included

| # | Chart Type   | Insight                                      |
|---|-------------|----------------------------------------------|
| 1 | Pie Chart    | Above vs Below Median extent distribution    |
| 2 | Histogram    | Frequency distribution of extent values      |
| 3 | Line Chart   | Annual trend + 5-year rolling average        |
| 4 | Bar Chart    | Average extent per decade                    |
| 5 | Scatter Plot | Year vs extent with trend line               |
| 6 | Box Plot     | Spread and outliers by era                   |
| 7 | Heatmap      | Correlation matrix of engineered features    |
| 8 | Area Chart   | Cumulative trend over time                   |
| 9 | Count Plot   | Number of observations per era               |
| 10| Violin Plot  | Probability density by era                   |
| ★ | Pair Plot    | Bonus: Multi-feature relationship grid       |

---

## 🎛️ Filters (All Linked to Every Chart)

- **Year Range Slider** — Filter data by year range
- **Extent Category** — Above/Below Median dropdown
- **Extent Range Slider** — Numerical range filter
- **Era Multi-Select** — Pre-1990, 1990s, 2000s, 2010s+
- **Search / Text** — Filter by year, era, or decade keyword
- **Reset Button** — Resets all filters to default

---

## 💡 Key Insights

1. **Dramatic decline post-2007:** Arctic ice extent dropped sharply after 2007, with 2012 recording the lowest extent (3.387 million km²).
2. **1980s were peak years:** The 1980s decade shows the highest average extent, indicating stable, cooler Arctic conditions.
3. **Strong negative correlation with year:** As years increase, ice extent decreases — clear evidence of climate change impact.
4. **High variability in early years:** Pre-1990 data shows natural oscillations, while post-2010 data shows consistently lower values.
5. **5-year rolling average confirms trend:** The rolling average smooths out annual variability and clearly shows a downward trajectory.

---

## 🛠️ Tech Stack

| Tool       | Purpose                          |
|------------|----------------------------------|
| Python 3.x | Core language                    |
| Pandas     | Data loading, cleaning, analysis |
| NumPy      | Numerical computations           |
| Matplotlib | Core chart rendering             |
| Seaborn    | Statistical visualization        |
| Streamlit  | Interactive dashboard framework  |
