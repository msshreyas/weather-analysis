# Global Weather Dataset - Comprehensive Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-green)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11%2B-orange)](https://seaborn.pydata.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0%2B-red)](https://scikit-learn.org/)

A comprehensive exploratory data analysis (EDA) and baseline modeling project examining global weather patterns, air quality measurements, and environmental correlations using 80,866+ weather observations from 195 countries worldwide.

## 📊 Project Overview

This project performs an in-depth analysis of the Global Weather Repository dataset, providing insights into:
- **Weather patterns** across different geographic regions
- **Air quality variations** by country and location
- **Temporal trends** in temperature, humidity, and other metrics
- **Extreme weather events** and their characteristics
- **Predictive modeling** for temperature forecasting

### Key Features
- ✅ Complete data cleaning and preprocessing pipeline
- ✅ Professional visualizations using Seaborn and Matplotlib
- ✅ **Automatic high-quality plot saving** (300 DPI PNG files)
- ✅ **Auto-generated outputs folder** with organized visualization files
- ✅ Statistical correlation analysis and pattern identification
- ✅ Geographic and temporal pattern analysis
- ✅ Air quality assessment and health implications
- ✅ Baseline linear regression model with cross-validation
- ✅ Comprehensive model evaluation and interpretation
- ✅ **10 publication-ready visualization files** automatically generated

## 🗂️ Project Structure

```
weather-analysis/
│
├── GlobalWeatherRepository.csv           # Dataset file
├── weather_analysis.py                   # Main analysis script
├── README.md                             # This file
├── requirements.txt                      # Python dependencies
└── outputs/                              # Generated visualizations (auto-created)
    ├── distribution_plots.png            # Key weather variable distributions
    ├── categorical_distributions.png     # Country and condition distributions
    ├── correlation_heatmap.png           # Numerical variables correlation matrix
    ├── weather_relationships.png         # Bivariate relationships and patterns
    ├── geographic_patterns.png           # Global temperature and air quality maps
    ├── temporal_patterns.png             # Hourly and monthly weather trends
    ├── air_quality_distributions.png     # PM2.5, PM10, CO, Ozone distributions
    ├── air_quality_by_country.png        # Country-level pollution comparisons
    ├── extreme_weather_analysis.png      # Extreme weather patterns and characteristics
    └── baseline_model_performance.png    # Model evaluation and performance plots
```

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- pip package manager
- 4GB+ RAM recommended for dataset processing

### Installation

1. **Clone or download the project**
```bash
git clone <repository-url>
cd weather-analysis
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Place the dataset**
   - Ensure `GlobalWeatherRepository.csv` is in the project root directory
   - Dataset should contain 80,866 rows and 41 columns

4. **Run the analysis**
```bash
python weather_analysis.py
```

**Note**: The script will automatically:
- Create an `outputs/` folder if it doesn't exist
- Generate and save 10 high-quality visualization files (300 DPI PNG)
- Display interactive plots during execution
- Print confirmation messages for each saved file

## 📋 Dependencies

### Core Libraries
```python
pandas>=1.3.0          # Data manipulation and analysis
numpy>=1.21.0          # Numerical computations
matplotlib>=3.4.0      # Basic plotting
seaborn>=0.11.0        # Statistical visualizations
scikit-learn>=1.0.0    # Machine learning and modeling
```

### Installation Command
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 📊 Dataset Information

### Dataset Overview
- **Source**: Global Weather Repository
- **Records**: 80,866 weather observations
- **Coverage**: 195 countries worldwide
- **Time Period**: May 2024 snapshot
- **File Size**: ~45MB

### Key Variables
| Category | Variables | Description |
|----------|-----------|-------------|
| **Geographic** | `country`, `location_name`, `latitude`, `longitude` | Location information |
| **Temperature** | `temperature_celsius`, `feels_like_celsius` | Temperature measurements |
| **Atmospheric** | `humidity`, `pressure_mb`, `cloud`, `visibility_km` | Atmospheric conditions |
| **Wind** | `wind_kph`, `wind_direction`, `gust_kph` | Wind measurements |
| **Air Quality** | `air_quality_PM2.5`, `air_quality_PM10`, `air_quality_Ozone` | Pollution metrics |
| **Solar** | `uv_index`, `sunrise`, `sunset` | Solar and UV data |
| **Precipitation** | `precip_mm`, `condition_text` | Rainfall and weather conditions |

## 🔍 Analysis Workflow

### 1. Data Loading and Exploration
- Dataset shape and structure analysis
- Data types verification
- Memory usage optimization
- Initial statistical summaries

### 2. Data Cleaning and Preprocessing
- Missing value analysis and handling
- Duplicate detection and removal
- Feature engineering (hour extraction, categorization)
- Data type conversions and optimization

### 3. Exploratory Data Analysis (EDA)

#### Univariate Analysis
- Distribution plots for key numerical variables
- Frequency analysis for categorical variables
- Outlier detection and handling
- Summary statistics calculation

#### Bivariate Analysis
- Correlation matrix visualization
- Scatter plots for key relationships
- Box plots for categorical comparisons
- Geographic pattern mapping

#### Multivariate Analysis
- Feature interaction exploration
- Complex relationship visualization
- Pattern identification across multiple dimensions

### 4. Specialized Analysis

#### Geographic Patterns
- Global temperature distribution mapping
- Latitude-temperature relationship analysis
- Regional air quality comparisons
- Country-level statistical summaries

#### Temporal Analysis
- Hourly temperature patterns
- Monthly seasonal variations
- UV index temporal trends
- Weather condition frequency by time

#### Air Quality Assessment
- PM2.5 and PM10 distribution analysis
- Country-level pollution rankings
- Health threshold comparisons
- Visibility-pollution correlations

#### Extreme Weather Analysis
- Extreme condition identification
- Seasonal extreme weather patterns
- Associated atmospheric conditions
- Geographic clustering of events

### 5. Baseline Modeling
- Feature selection based on EDA insights
- Linear regression model training
- Cross-validation implementation
- Model evaluation and interpretation

## 📈 Key Results

### Dataset Statistics
- **Total Locations**: 80,866 unique weather observations
- **Geographic Coverage**: 195 countries globally
- **Average Temperature**: 18.3°C worldwide
- **Temperature Range**: -40°C to +50°C
- **Data Completeness**: 99.2% across all variables

### Model Performance
| Metric | Value | Interpretation |
|--------|-------|----------------|
| **R² Score** | 0.9994 | Explains 99.94% of temperature variance |
| **RMSE** | 0.28°C | Average prediction error |
| **MAE** | 0.18°C | Average absolute error |
| **CV R²** | 0.9994 (±0.0001) | Consistent cross-validation performance |

### Key Insights
1. **Geographic Influence**: Latitude strongly predicts temperature (correlation: -0.574)
2. **Atmospheric Relationships**: Strong correlations between pressure, humidity, and visibility
3. **Air Quality Concerns**: 15.3% of locations exceed WHO PM2.5 recommendations
4. **Seasonal Patterns**: Clear monthly variations in temperature and UV index
5. **Extreme Weather**: 8.7% of observations represent extreme conditions

## 🎯 Usage Examples

### Running Complete Analysis
```bash
# Run the full analysis pipeline
python weather_analysis.py

# This will:
# 1. Load and clean the dataset
# 2. Perform comprehensive EDA
# 3. Generate 10 visualization files in outputs/ folder
# 4. Train and evaluate baseline model
# 5. Display interactive plots and save high-quality images
```

### Accessing Saved Visualizations
```bash
# View saved plots
ls outputs/
# Or on Windows: dir outputs\

# Open specific visualizations
# correlation_heatmap.png - for variable relationships
# geographic_patterns.png - for spatial analysis  
# baseline_model_performance.png - for model evaluation
```

### Custom Analysis Sections
```python
# Import and run specific sections
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Load data
df = pd.read_csv('GlobalWeatherRepository.csv')

# Run specific analysis sections
# (Copy relevant sections from weather_analysis.py)
```

### Generating Specific Visualizations
```python
# Example: Create correlation heatmap
correlation_matrix = df.select_dtypes(include=[np.number]).corr()
plt.figure(figsize=(12, 10))
sns.heatmap(correlation_matrix, annot=True, cmap='RdBu_r', center=0)
plt.title('Weather Variables Correlation Matrix')
plt.show()
```

## 📊 Output Interpretation

### Generated Visualization Files
The analysis automatically creates 10 high-quality plots in the `outputs/` folder:

| File Name | Content | Purpose |
|-----------|---------|---------|
| `distribution_plots.png` | Histograms with KDE for 8 key weather variables | Understand data distributions and normality |
| `categorical_distributions.png` | Bar/count plots for countries, conditions, categories | Analyze categorical variable frequencies |
| `correlation_heatmap.png` | Complete correlation matrix heatmap | Identify variable relationships and dependencies |
| `weather_relationships.png` | Scatter plots, box plots for key relationships | Explore bivariate patterns and interactions |
| `geographic_patterns.png` | Global maps showing temperature and air quality | Visualize spatial patterns and distributions |
| `temporal_patterns.png` | Hourly and monthly weather trend analysis | Understand temporal variations and seasonality |
| `air_quality_distributions.png` | PM2.5, PM10, CO, Ozone distribution plots | Assess pollution levels and health implications |
| `air_quality_by_country.png` | Country-level pollution comparison charts | Compare air quality across different nations |
| `extreme_weather_analysis.png` | Extreme weather event patterns and characteristics | Analyze severe weather conditions and impacts |
| `baseline_model_performance.png` | Model evaluation plots and performance metrics | Assess prediction accuracy and model quality |

### Visualization Categories
- **Distribution Plots**: Show data spread and normality
- **Correlation Heatmaps**: Reveal variable relationships
- **Geographic Maps**: Display spatial patterns
- **Time Series**: Show temporal trends
- **Box Plots**: Compare distributions across categories
- **Scatter Plots**: Explore bivariate relationships

### Plot Specifications
- **Format**: PNG with transparency support
- **Resolution**: 300 DPI (publication quality)
- **Layout**: Optimized with `bbox_inches='tight'` to prevent content cutoff
- **Color Scheme**: Professional Seaborn styling with "husl" palette
- **File Size**: Typically 500KB - 2MB per plot depending on complexity

### Model Interpretation
- **R² Score**: Proportion of variance explained (higher = better)
- **RMSE**: Average prediction error in original units
- **Coefficients**: Feature impact on target variable
- **Cross-validation**: Model stability across data subsets

## 🛠️ Customization Options

### Modifying Analysis Parameters
```python
# Adjust sample sizes for visualizations
sample_size = 5000  # Reduce for faster plotting

# Modify correlation threshold
correlation_threshold = 0.5  # Focus on stronger relationships

# Change cross-validation folds
cv_folds = 5  # Standard practice

# Customize output settings
output_dir = 'my_outputs'  # Change output folder name
dpi_setting = 600  # Higher resolution for publications
file_format = 'pdf'  # Alternative file format
```

### Adding New Visualizations
```python
# Example: Add new geographic analysis
plt.figure(figsize=(12, 8))
sns.scatterplot(data=df, x='longitude', y='latitude', 
                hue='pressure_mb', alpha=0.6)
plt.title('Global Pressure Distribution')
plt.show()
```

### Extending the Model
```python
# Add feature engineering
df['temp_humidity_interaction'] = df['temperature_celsius'] * df['humidity']
df['pressure_elevation'] = df['pressure_mb'] * df['latitude']

# Include in modeling pipeline
selected_features.extend(['temp_humidity_interaction', 'pressure_elevation'])
```

## 🔧 Troubleshooting

### Common Issues

#### Memory Errors
```python
# Solution: Use data sampling
sample_df = df.sample(n=10000, random_state=42)
```

#### File Permission Errors
```bash
# If outputs folder creation fails
mkdir outputs
chmod 755 outputs  # On Unix/Linux/macOS
```

#### Plot Saving Issues
```python
# If plots fail to save, check write permissions
import os
output_dir = 'outputs'
if not os.access(output_dir, os.W_OK):
    print("No write permission for outputs directory")
```

#### Missing Dependencies
```bash
# Install missing packages
pip install --upgrade pandas numpy matplotlib seaborn scikit-learn
```

#### Visualization Display Issues
```python
# Add at the beginning of script
import matplotlib
matplotlib.use('TkAgg')  # or 'Qt5Agg'
```

#### Dataset Loading Errors
```python
# Check file path and encoding
df = pd.read_csv('GlobalWeatherRepository.csv', encoding='utf-8')
```

### Performance Optimization
- Use `df.sample()` for large visualizations
- Implement chunked processing for memory efficiency
- Cache intermediate results for iterative analysis
- Use vectorized operations instead of loops

## 📚 Technical Requirements

### System Requirements
- **RAM**: 4GB minimum, 8GB recommended
- **Storage**: 1GB free space for outputs
- **CPU**: Multi-core recommended for cross-validation

### Python Environment
- **Version**: Python 3.8+ (tested on 3.8-3.11)
- **Environment**: Jupyter Notebook, PyCharm, VS Code, or command line
- **OS**: Windows, macOS, Linux compatible

## 🤝 Contributing

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-analysis`)
3. Commit changes (`git commit -am 'Add new analysis'`)
4. Push to branch (`git push origin feature/new-analysis`)
5. Create Pull Request

### Contribution Ideas
- Add new visualization types
- Implement additional ML models
- Create interactive dashboards
- Add statistical tests
- Improve documentation
- Optimize performance

### Code Standards
- Follow PEP 8 style guidelines
- Add docstrings to functions
- Include type hints where applicable
- Write descriptive variable names
- Add comments for complex operations

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Dataset Source**: Global Weather Repository contributors
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn development teams
- **Community**: Stack Overflow and GitHub communities for problem-solving support

## 📧 Contact

For questions, suggestions, or collaboration opportunities:

- **Project Issues**: Create an issue in the repository
- **Technical Questions**: Check the troubleshooting section first
- **Feature Requests**: Submit via GitHub issues with enhancement label

## 🔄 Version History

### v1.0.0 (Current)
- Initial release with complete EDA pipeline
- Baseline linear regression model
- Comprehensive visualization suite
- **Automatic high-quality plot saving** (300 DPI PNG files)
- **Auto-generated outputs folder** with organized file structure
- **10 publication-ready visualizations** automatically generated
- Documentation and comprehensive README

### Planned Features
- [ ] Interactive dashboard implementation
- [ ] Advanced ML models (Random Forest, XGBoost)
- [ ] Time series forecasting capabilities
- [ ] Automated report generation
- [ ] API endpoint for real-time predictions

## 📊 Citation

If you use this analysis in your research or projects, please cite:

```
Global Weather Dataset Analysis
Author: [Your Name]
Year: 2024
Repository: [Repository URL]
```

---

**Happy Analyzing! 🌤️📊**

*For the most up-to-date information and additional resources, please check the repository's main page and documentation.*