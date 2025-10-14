````markdown
# Customer Segmentation Analysis

## Description

This project performs an in-depth customer segmentation analysis on a transactional dataset online retail store. The primary goal is to identify best performing clustering algorithm on the dataset, distinct customer groups based on their purchasing behavior, enabling targeted marketing strategies and personalized customer experiences.

The analysis involves comprehensive data cleaning, exploratory data analysis (EDA), feature engineering, and the application of various clustering algorithms. The project culminates in the evaluation and selection of the most suitable clustering model for customer segmentation.

## Dataset

The dataset used in this project is the **"Online Retail"** dataset, which contains transactional data. The dataset is provided as `online_retail.csv`.

## Installation

To run this project, you need Python and Jupyter Notebook installed. Install the required libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kneed hdbscan umap-learn plotly
````

## Usage

1. Clone the repository:

```bash
git clone https://github.com/your-username/customer-segmentation.git
```

2. Navigate to the project directory:

```bash
cd customer-segmentation
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open the `cs_without_output.ipynb` notebook and run the cells sequentially.

## Project Structure

The project is organized into a single Jupyter Notebook (`cs_without_output.ipynb`) and is divided into the following tasks:

### Task 1: Initial Data Inspection and Cleaning

* Load the dataset.
* Handle missing and duplicate values.
* Perform initial data visualization to understand variable distributions and relationships.

### Task 2: Data Preprocessing and Feature Engineering

* Aggregate data by invoice, stock code, and customer ID.
* Disambiguate transaction types (e.g., sales, returns, adjustments).
* Categorize item types (products, discounts, shipping, etc.).
* Handle anomalous price values.
* Extract time-based features from the invoice date.

### Task 3: Country-Specific Analysis (India)

* Split the dataset by country.
* Analyze India-specific sales trends, top products, and customer behavior.
* Categorize product prices into different ranges.

### Customer Segmentation

* Apply various clustering algorithms to segment customers.
* Evaluate clustering models using metrics like Silhouette Score, Calinski-Harabasz Score, and Davies-Bouldin Score.
* Visualize resulting clusters.

## Methodology

### Data Cleaning and Preprocessing

* Handle missing values, duplicates, and inconsistencies.
* Engineer new features, including:

  * `Transaction_Type` – classifies transactions into sales, returns, and adjustments.
  * `Item_Type` – categorizes items into products, discounts, shipping, etc.
  * Time-based features: year, month, day, day of week, and hour of transaction.

### Exploratory Data Analysis (EDA)

* Visualize key distributions such as `Quantity` and `Price`.
* Identify top-selling products and countries with the highest orders.
* Analyze sales trends over time.

### Customer Segmentation

* Apply clustering algorithms including:

  * K-Means & Mini-Batch K-Means
  * Birch
  * DBSCAN
  * Agglomerative Clustering
  * Affinity Propagation
  * Mean Shift
  * Spectral Clustering
  * OPTICS
  * Gaussian Mixture Models (GMM)
  * HDBSCAN
* Evaluate model performance with standard clustering metrics to select the best segmentation model.

## Results

Key insights from the analysis include:

* Best performing Clustering Algorithm.
* Identification of the most valuable customers.
* Understanding purchasing patterns of different customer segments.
* Insights into popular products and peak purchasing times.

These results can be leveraged to:

* Develop targeted marketing campaigns.
* Improve customer relationship management.
* Optimize inventory management.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your proposed changes.
