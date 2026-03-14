# 🍽️ Zomato Data Analysis

Exploratory Data Analysis (EDA) of a Zomato restaurant dataset to uncover trends in restaurant types, customer preferences, ratings, ordering modes, and spending behaviour.

---

## 📌 Project Overview

This project performs EDA on a dataset of 148 Zomato-listed restaurants. The analysis explores how restaurants are categorized, what influences their ratings, how customers order, and what they typically spend — providing actionable insights into the restaurant industry.

---

## 📂 Repository Structure

```
Zomato-Data-Analysis/
│
├── Zomato_Data_Analysis.ipynb   # Main Jupyter Notebook with full analysis
├── Zomato_data.csv              # Dataset used for the analysis
└── README.md                    # Project documentation
```

---

## 📊 Dataset

**File:** `Zomato_data.csv`  
**Rows:** 148  
**Columns:** 7

| Column | Description |
|---|---|
| `name` | Name of the restaurant |
| `online_order` | Whether the restaurant accepts online orders (Yes/No) |
| `book_table` | Whether table booking is available (Yes/No) |
| `rate` | Customer rating out of 5 (e.g., `4.1/5`) |
| `votes` | Total number of votes received |
| `approx_cost(for two people)` | Approximate cost for two people (in INR) |
| `listed_in(type)` | Category of the restaurant (Buffet, Cafes, Dining, Other) |

---

## 🔍 Analysis Performed

- **Data Loading & Cleaning** — Loading CSV, fixing the `rate` column by stripping the `/5` string and converting to float
- **Dataset Structure** — Shape, data types, and null value check
- **Type of Restaurants** — Count plot of restaurant categories
- **Votes by Restaurant Type** — Line plot of total votes per category
- **Rating Distribution** — Histogram of restaurant ratings
- **Avg Order Spending by Couples** — Count plot of approximate cost for two
- **Online vs Offline Order Ratings** — Box plot comparing ratings by ordering mode
- **Online Order vs Restaurant Type** — Heatmap showing distribution across categories

---

## 💡 Key Insights

- **Dining** restaurants are the most common category on Zomato.
- **Dining** restaurants receive the maximum number of votes from customers.
- Most restaurants have ratings between **3.5 and 4.0**.
- The majority of couples prefer restaurants with an approximate cost of **₹300**.
- Restaurants accepting **online orders tend to receive higher ratings** compared to offline-only restaurants.
- The heatmap reveals that **Dining restaurants overwhelmingly prefer offline ordering**, while Cafes have a higher proportion of online orders.

---

## 🛠️ Technologies Used

- **Python 3**
- **Pandas** — Data manipulation and cleaning
- **NumPy** — Numerical operations
- **Matplotlib** — Static visualizations
- **Seaborn** — Statistical plots and heatmaps
- **Google Colab** — Development environment

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/Zomato-Data-Analysis.git
cd Zomato-Data-Analysis
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the notebook
Open `Zomato_Data_Analysis.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.

> **Note:** If running on Google Colab, upload `Zomato_data.csv` to the session storage and ensure the file path matches:
> ```python
> dataframe = pd.read_csv('/content/Zomato data .csv')
> ```

---

## 📈 Visualizations Included

| Chart | Purpose |
|---|---|
| Count Plot | Restaurant type distribution |
| Line Plot | Total votes by restaurant type |
| Histogram | Rating frequency distribution |
| Count Plot | Spending distribution for couples |
| Box Plot | Online vs offline order ratings |
| Heatmap | Online ordering behaviour across restaurant types |

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request for improvements, additional analyses, or bug fixes.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙏 Acknowledgements

- Dataset sourced from [Zomato](https://www.zomato.com/) restaurant listings
- Inspired by real-world food-tech and consumer behaviour analytics
