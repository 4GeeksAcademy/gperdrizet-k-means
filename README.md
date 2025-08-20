# California Housing Market Clustering with K-means

[![Codespaces Prebuilds](https://github.com/4GeeksAcademy/gperdrizet-k-means/actions/workflows/codespaces/create_codespaces_prebuilds/badge.svg)](https://github.com/4GeeksAcademy/gperdrizet-k-means/actions/workflows/codespaces/create_codespaces_prebuilds)

A comprehensive machine learning project demonstrating unsupervised clustering with K-means and supervised classification on California housing market data. This project combines geographic and economic data analysis to identify distinct housing market segments and build predictive models.


## Project Overview

This project analyzes California housing data to discover natural market segments using K-means clustering, then builds supervised models to predict cluster membership. The analysis focuses on **geographic location** (latitude, longitude) and **economic factors** (median income) to provide hands-on experience with:

- Unsupervised machine learning (K-means clustering)
- Data preprocessing and feature scaling
- Geographic and economic data visualization
- Supervised classification model development
- Cross-validation and model evaluation
- 2D and 3D data visualization techniques


## Getting Started

### Option 1: GitHub Codespaces (Recommended)

1. **Fork the Repository**
   - Click the "Fork" button on the top right of the GitHub repository page
   - 4Geeks students: set 4GeeksAcademy as the owner - 4Geeks pays for your codespace usage. All others, set yourself as the owner
   - Give the fork a descriptive name. 4Geeks students: I recommend including your GitHub username to help in finding the fork if you loose the link
   - Click "Create fork"
   - 4Geeks students: bookmark or otherwise save the link to your fork

2. **Create a GitHub Codespace**
   - On your forked repository, click the "Code" button
   - Select "Create codespace on main"
   - If the "Create codespace on main" option is grayed out - go to your codespaces list from the three-bar menu at the upper left and delete an old codespace
   - Wait for the environment to load (dependencies are pre-installed)

3. **Start Working**
   - Open `notebooks/mvp.ipynb` in the Jupyter interface for the assignment
   - Follow the step-by-step instructions in the notebook
   - Reference `notebooks/solution.ipynb` for the complete implementation

### Option 2: Local Development

1. **Prerequisites**
   - Git
   - Python >= 3.10

2. **Fork the repository**
   - Click the "Fork" button on the top right of the GitHub repository page
   - Optional: give the fork a new name and/or description
   - Click "Create fork"

3. **Clone the repository**
   - From your fork of the repository, click the green "Code" button at the upper right
   - From the "Local" tab, select HTTPS and copy the link
   - Run the following commands on your machine, replacing `<LINK>` and `<REPO_NAME>`

   ```bash
   git clone <LINK>
   cd <REPO_NAME>
   ```

4. **Set Up Environment**

   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

5. **Launch Jupyter & start the notebook**
   ```bash
   jupyter notebook notebooks/mvp.ipynb
   ```


## Project Structure

```
├── .devcontainer/      # Development container configuration
├── data/               # Data storage directory
├── models/             # Model storage directory
│
├── notebooks/          # Jupyter notebook directory
│   ├── functions.py    # Helper functions for analysis
│   ├── mvp.ipynb       # Assignment notebook (start here)
│   └── solution.ipynb  # Complete solution notebook
│
├── .gitignore          # Files/directories not tracked by git
├── LICENSE             # Project license
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

## Dataset

The project uses California housing data from the 4GeeksAcademy K-means tutorial repository. The dataset contains housing market information with the following key features used for clustering:

- **MedInc**: Median income in the area (economic factor)
- **Latitude**: Geographic coordinate (north-south position)  
- **Longitude**: Geographic coordinate (east-west position)

The dataset provides 20,640 housing records across California, offering rich geographic and economic diversity for clustering analysis.

**Data Source**: https://raw.githubusercontent.com/4GeeksAcademy/k-means-project-tutorial/main/housing.csv


## Learning Objectives

1. **Data Loading & Preprocessing**: Load remote data, save local copies, and prepare features
2. **Exploratory Data Analysis**: Analyze feature distributions and correlations
3. **Data Preparation**: Train-test splitting and feature scaling with MinMaxScaler
4. **Unsupervised Learning**: Apply K-means clustering to identify market segments
5. **Data Visualization**: Create 2D geographic plots and 3D scatter visualizations
6. **Supervised Learning**: Build classification models to predict cluster membership
7. **Model Evaluation**: Implement cross-validation and assess model performance
8. **Market Analysis**: Interpret clustering results in real-world context


## Technologies Used

- **Python 3.11**: Core programming language
- **Pandas 2.3.1**: Data manipulation and analysis
- **Scikit-learn 1.7.1**: Machine learning algorithms and preprocessing
- **Matplotlib 3.10.3**: Static data visualization
- **Seaborn 0.13.2**: Statistical data visualization
- **Plotly 6.0.1**: Interactive 3D visualizations
- **NumPy 2.3.2**: Numerical computing
- **Jupyter 1.1.1**: Interactive development environment
- **GitHub Codespaces**: Cloud-based development environment
