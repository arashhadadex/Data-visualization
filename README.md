# Pandas DataFrame Visualization in One Line of Code
Learn how to use Pandas .plot() for fast DataFrame visualization, like histograms, scatter plots, heatmaps, and Seaborn integration with real-world Python examples.

This guide uses the California Housing dataset (20,000+ rows) to show real-world visualization patterns. You'll also see where Seaborn fits for statistical plots and when to reach for Plotly to add interactivity.

---

## Load the Dataset
```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the California Housing dataset (~20,640 rows)
url = "https://raw.githubusercontent.com/ageron/handson-ml/master/datasets/housing/housing.csv"
df = pd.read_csv(url)
```
---

## Histograms: Check Your Distributions First
```
df['median_house_value'].plot(
    kind='hist',
    bins=50,
    figsize=(10, 6),
    color='steelblue',
    edgecolor='white',
    title='Distribution of Median House Values (California Housing Dataset)'
)
```
---

## Line plots
```
df_sorted.plot(
    x='median_income',
    y='median_house_value',
    kind='line',
    figsize=(10, 6),
    color='seagreen',
    alpha=0.6,
    title='Median House Value vs. Median Income'
)
```
---
## Bar plots
## Correlation Heatmap
## Scatter plots
## Pair plots with seaborn
## Box plots
## Plotly
---
Start with a histogram. Then a scatter plot. Then a heatmap. By the time you've run those three on a new dataset, you'll already know more about it than most people who've only read the column names.

---
## Requirements

No installation needed if you run the notebook in Google Colab. All libraries used are pre-installed in Colab:
```
pandas
matplotlib
seaborn plotly
```
---
## To run locally:
```
pip install pandas numpy
jupyter notebook
```
---

## Repository Structure
```
├── visualization.ipynb 
└── README.md
```
---
📖 Related Article

This notebook is the companion code for the article:

https://datatodeploy.com/exploring-pandas-dataframe-visualization-in-one-line-of-code/

---
## Contributing

Found a bug or want to add another trick? Feel free to open an issue or submit a pull request.

---

## License

This project is open source and available under the MIT License.
