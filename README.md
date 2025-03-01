# Public Transport Accessibility in Smart Cities

This project demonstrates the application of **Principal Component Analysis (PCA)** for dimensionality reduction using a dataset on public transport accessibility in smart cities. The goal is to simplify and visualize the high-dimensional data in a 2D space while retaining as much information as possible.

---

## Dataset Description
The dataset contains information about public transport facilities in various cities. The columns include:

- **City Name**: Name of the city.
- **Type Of Bus (AC / Non AC)**: Indicates whether the bus is air-conditioned or not.
- **No. of buses of that type**: Number of buses of the specified type.
- **No. of bus terminals**: Number of bus terminals in the city.
- **No. of bus stands**: Number of bus stands in the city.
- **No. of bus stops**: Number of bus stops in the city.

---

## Project Workflow

### 1. Preprocessing
- Numerical features are selected for analysis.
- Missing or non-numeric values are handled by dropping them.

### 2. Standardization
- The data is standardized using `StandardScaler` to ensure all features contribute equally to PCA.

### 3. Dimensionality Reduction
- PCA reduces the dataset dimensions from 4 to 2.
- The first two principal components capture the most variance in the data.

### 4. Visualization
- The reduced dataset is visualized in a 2D scatter plot where each point represents a city.

---

## Requirements
To run the code, you need the following Python libraries installed:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`

You can install them using:
```bash
pip install pandas numpy scikit-learn matplotlib
```

---

## Usage

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/transport-pca-project.git
cd transport-pca-project
```

### Step 2: Add the Dataset
Place the dataset file (`public-transport-accessibility-smart-cities.csv`) in the project directory.

### Step 3: Run the Script
Execute the Python script:
```bash
python pca_analysis.py
```

### Step 4: View the Output
- A scatter plot will be displayed showing the cities in the 2D PCA-reduced space.

---

## Example Output
Below is an example of the 2D scatter plot generated by PCA:

![PCA Visualization](example_pca_plot.png)

---

## File Structure
```
transport-pca-project/
├── public-transport-accessibility-smart-cities.csv  # Dataset file
├── pca_analysis.py                                 # Python script for PCA
├── README.md                                       # Project documentation
└── example_pca_plot.png                           # Example visualization
```

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

