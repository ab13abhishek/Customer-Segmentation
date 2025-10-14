# Customer Segmentation Analysis 📊

![Python](https://img.shields.io/badge/python-3.11-blue?logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)

## 🔍 Project Overview

This project performs **customer segmentation** on a online retail dataset to identify distinct customer groups based on their purchasing behavior.
The insights can be used to:
- Best performing clustering algorithm.
- Enable targeted marketing campaigns.
- Personalize customer experiences.
- Optimize inventory and sales strategies.

The analysis includes **data cleaning**, **exploratory data analysis (EDA)**, **feature engineering**, and **clustering using multiple algorithms**.

## 📁 Dataset

The dataset used is **"Online Retail"**, containing transactional data for a registered non-store online retail.  

- File: `online_retail.csv`
- Columns include: `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`.

## ⚙️ Installation

1. Ensure you have **Python** and **Jupyter Notebook** installed.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kneed hdbscan umap-learn plotly

## 🚀 Usage

1. Clone the repository:

```bash
git clone https://github.com/ab13abhishek/Customer-Segmentation.git
```

2. Navigate to the project directory:

```bash
cd Customer-Segmentation
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open the notebook `cs_without_output.ipynb` and run cells sequentially.

## 📊 Project Structure

| Task                                     | Description                                                                       |
| ---------------------------------------- | --------------------------------------------------------------------------------- |
| **1. Data Cleaning**                     | Load data, handle missing values and duplicates, visualize distributions.         |
| **2. Feature Engineering**               | Aggregate data, classify transactions and item types, create time-based features. |
| **3. Country-Specific Analysis (India)** | Analyze India-specific trends, visualize top products, categorize prices.         |
| **4. Customer Segmentation**             | Apply clustering algorithms, evaluate metrics, visualize clusters.                |

## 🛠 Methodology

### 1. Data Cleaning & Preprocessing

* Handle missing values and duplicates.
* Engineer features:

  * `Transaction_Type` – Sales, Returns, Adjustments
  * `Item_Type` – Products, Discounts, Shipping
  * Time features – Year, Month, Day, DayOfWeek, Hour

### 2. Exploratory Data Analysis (EDA)

* Visualize distributions of `Quantity` and `Price`.
* Identify top-selling products and countries.
* Analyze sales trends over time.

### 3. Customer Segmentation

* Algorithms used:

  * **K-Means**, **Mini-Batch K-Means**
  * **Birch**, **DBSCAN**, **OPTICS**, **Agglomerative Clustering**
  * **Affinity Propagation**, **Mean Shift**, **Spectral Clustering**
  * **Gaussian Mixture Models (GMM)**, **HDBSCAN**
* Metrics for evaluation: **Silhouette Score**, **Calinski-Harabasz Score**, **Davies-Bouldin Score**

## 📈 Results

Key insights:

* Best Perfoming Clustering Algorithm.
* Identified **most valuable customers**.
* Discovered **distinct purchasing patterns**.
* Revealed **popular products** and **peak purchasing times**.

These insights can guide **marketing campaigns, CRM strategies, and inventory planning**.

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create your branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.
