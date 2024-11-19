**McDonald's Market Segmentation Analysis**

This repository contains an implementation of market segmentation analysis based on the McDonald's case study. The analysis involves exploratory data analysis, preprocessing, clustering, and advanced stability and profiling techniques. The dataset is sourced from a case study on fast food preferences.

---

## **Dataset**

The dataset (`mcdonalds.csv`) contains responses to various questions regarding customer preferences for McDonald's products. The columns represent binary responses (`Yes` or `No`) to attributes or features about the food and services. It includes:

- **Features (Columns 1-11):** Questions about preferences or opinions on specific attributes (e.g., taste, quality, healthiness).
- **Other Columns (if applicable):** Demographic or other auxiliary data (e.g., age, income, etc.).

### **Dataset Summary**
| Column Name       | Description                                  | Example Values   |
|--------------------|----------------------------------------------|------------------|
| `Taste`           | Preference for taste                        | Yes/No           |
| `HealthyOptions`  | Availability of healthy food options         | Yes/No           |
| `Speed`           | Perception of service speed                 | Yes/No           |
| ...               | ...                                          | ...              |

---

## **Program Workflow**

This repository provides Python code to replicate the analysis described in the McDonald's segmentation case study using techniques such as PCA, k-means clustering, and segment profiling.

### **Steps in the Analysis**
1. **Load Data:** Load and explore the dataset to understand its structure.
2. **Data Preprocessing:** Convert categorical data (`Yes`/`No`) to binary format (`1`/`0`).
3. **Principal Component Analysis (PCA):** Reduce dimensionality for easier visualization and clustering.
4. **k-Means Clustering:** Identify customer segments by grouping similar preferences.
5. **Cluster Stability Analysis:** Evaluate the robustness of clustering results using bootstrapping.
6. **Visualization:** Visualize clusters in PCA space and interpret the results.
7. **Segment Profiling:** Understand the key characteristics of each customer segment.
8. **Statistical Testing:** Test the significance of differences across clusters.

---

## **Requirements**

The following Python libraries are required:
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
- `scipy`

You can install them using:
```bash
pip install pandas numpy matplotlib scikit-learn scipy
```

---

## **Usage**

### **Run the Program**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/mcdonalds-segmentation-analysis.git
   cd mcdonalds-segmentation-analysis
   ```
2. Ensure the `mcdonalds.csv` file is in the root directory.
3. Open the Jupyter notebook or Python script in your environment (e.g., Google Colab).
4. Run the code sequentially to replicate the analysis.

### **Google Colab Instructions**
1. Upload the dataset to your Colab environment.
2. Copy the Python code into a Colab notebook.
3. Replace `"mcdonalds.csv"` with the correct file path.

---

## **Output**

### **Key Outputs**
- **Scree Plot:** Displays the variance explained by each principal component.
- **Cluster Visualizations:** Scatter plot of customer segments in PCA space.
- **Cluster Stability:** Evaluation of clustering robustness using Adjusted Rand Index.
- **Segment Profiles:** Average feature preferences for each customer segment.

### **Example Visualizations**
1. Scree Plot: Helps determine the optimal number of principal components.
2. Cluster Centroid Bar Chart: Visualizes the feature importance for each cluster.
