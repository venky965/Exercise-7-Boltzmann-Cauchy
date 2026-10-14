# Exercise 8: Kohonen Self-Organizing Map (SOM)

## Customer Segmentation and Cluster Exploration System Using Mall Customers Dataset

### Objective
To develop a Self-Organizing Map (SOM)-based system for customer segmentation using the Mall Customers dataset. The system applies unsupervised learning to group customers based on their numerical attributes and explore customer clusters, prototypes, and outliers.

### Dataset
**Mall Customers Dataset (`Mall_Customers.csv`)**

The dataset typically contains customer information such as:
- Customer ID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1–100)

The numerical attributes are selected, missing values are handled, and the features are normalized using standardization before SOM training.

### Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

### Algorithm
The Kohonen Self-Organizing Map is an unsupervised neural network used to represent high-dimensional data on a lower-dimensional grid.

The implementation follows these steps:
1. Load the Mall Customers dataset.
2. Select numerical attributes and handle missing values.
3. Standardize the selected features.
4. Initialize the SOM weight vectors.
5. Find the Best Matching Unit (BMU) using Euclidean distance.
6. Update the winning neuron's weights and its neighboring neurons using competitive learning.
7. Analyze the resulting customer groups and cluster characteristics.

### Menu-Driven Features
1. **Customer Segmentation using SOM** – Assign customers to SOM neurons and visualize the segmentation.
2. **Best Matching Unit Explorer** – Find the BMU and distance for a selected customer.
3. **Dynamic Cluster Count Challenge** – Compare reference clustering results for different cluster counts.
4. **Customer Cluster Migration Analyzer** – Compare customer assignments between SOM configurations.
5. **Cluster Prototype Generator** – Display representative feature values for occupied SOM neurons.
6. **Outlier Customer Detector** – Identify customers with unusually large distances from their BMUs.
7. **SOM Cluster Quality Comparison** – Compare SOM configurations using quantization error.
8. **Exit** – Terminate the program.

### Project Structure
```text
Exercise_8_SOM/
├── Exercise_8_SOM.ipynb
├── Mall_Customers.csv
└── README.md
```

### Installation
Install the required libraries using:

```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

### How to Run
1. Download or clone this repository.
2. Place `Mall_Customers.csv` in the same directory as the notebook.
3. Open Jupyter Notebook.
4. Open `Exercise_8_SOM.ipynb`.
5. Run the notebook cells.
6. Select a menu option to explore the SOM system.

### Expected Outcome
The system demonstrates how a Self-Organizing Map can organize customers according to similarities in their numerical attributes. It supports customer segmentation, BMU exploration, cluster prototype analysis, outlier detection, and comparison of SOM configurations.

### Result
A menu-driven SOM customer segmentation and cluster exploration system is implemented using Python and the Mall Customers dataset. The system demonstrates unsupervised learning and competitive learning through a Kohonen Self-Organizing Map.
