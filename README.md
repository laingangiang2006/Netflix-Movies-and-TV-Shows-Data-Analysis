# Netflix Movies & TV Shows Data Analysis

Exploratory data analysis (EDA) of the Netflix Movies and TV Shows dataset, examining patterns in content popularity, genre distribution, vote engagement, and language representation.

## Repository Structure

```
Netflix-Movies-and-TV-Shows-Data-Analysis/
├── Figures/ # Charts (Figure_1 to Figure_6)
├── Netflix Movies & TV Shows Data Analysis.pptx # Full presentation
├── index.py # Main analysis script
└── README.md
```

---

## Dataset

- **Source:** [Kaggle – Netflix Movies and TV Shows Data Analysis](https://www.kaggle.com/datasets/nalisha/netflix-movies-and-tv-shows-data-analysis)
- **Size:** ~9,000+ titles
- **Key columns:** `Title`, `Genre`, `Original_Language`, `Popularity`, `Vote_Count`, `Vote_Average`, `Release_Date`
- [My Kaggle Code Notebook](https://www.kaggle.com/code/laingangiang2006/netflix-movies-tv-shows-data-analysis)

---

## Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python 3.x | Core language |
| pandas | Data manipulation |
| numpy | Numerical operations |
| matplotlib | Charting |
| seaborn | Statistical visualization |

---

## Methodology

1. Load dataset with `latin-1` encoding
2. Drop rows and columns with missing values
3. Cast `Vote_Count` to `int64`, `Vote_Average` to `float64`
4. Engineer categorical bins: `Popularity_Category`, `Vote_Count_Category`, `Vote_Average_Category`
5. Create dummy variables for `Genre` and `Original_Language`
6. Build pivot tables for aggregated analysis
7. Generate 6 visualizations across genre and language dimensions

---

## Visualizations

| Figure | Chart | Key Finding |
|--------|-------|-------------|
| Figure 1 | Average Popularity by Genre (Top 10) | Adventure leads at ~54, Horror trails at ~38 |
| Figure 2 | Movie Count by Genre (Top 10) | Drama dominates with ~3,700 titles |
| Figure 3 | Average Vote Count by Genre (Top 10) | Adventure (~2,300) and Sci-Fi (~2,200) top engagement |
| Figure 4 | Average Popularity by Language (Top 10) | Malayalam (ML) far outperforms at ~150 |
| Figure 5 | Movie Count by Language (Top 10) | English accounts for ~7,500 titles — 12× the next language |
| Figure 6 | Average Vote Count by Language (Top 10) | English leads at ~1,670 votes per title |

---

## Key Findings

- **Drama** is the highest-volume genre but ranks last in per-title vote engagement among the top 10
- **Adventure** is the strongest genre overall — top in both popularity and vote count
- **Malayalam (ML)** content achieves dramatically higher average popularity (~150) than any other language, including English (~42)
- **English** dominates volume (~7,500 titles) but only ranks 6th in average popularity
- **Science Fiction** achieves top-tier engagement despite a moderate catalog size

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/laingangiang2006/Netflix-Movies-and-TV-Shows-Data-Analysis.git

# Navigate into the project folder
cd Netflix-Movies-and-TV-Shows-Data-Analysis

# Install dependencies
pip install pandas numpy matplotlib seaborn

# Run the analysis
python index.py
```

> **Note:** Update the file path in `index.py` to point to your local copy of `mymoviedb (1).csv` before running.

---

## Presentation

The full analysis with slide-by-slide insights is available in:
`Netflix Movies & TV Shows  Data Analysis.pptx`

---

## License

This project is for educational purposes. Dataset credit: [Nalisha on Kaggle](https://www.kaggle.com/datasets/nalisha/netflix-movies-and-tv-shows-data-analysis).
