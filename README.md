# 🗽 NYC Taxi Trip Duration - Exploratory Data Analysis (EDA)

This project presents a detailed **Exploratory Data Analysis (EDA)** on the [NYC Taxi Trip Duration dataset]([https://www.kaggle.com/competitions/nyc-taxi-trip-duration/overview](https://github.com/akshaygrandhi123/Fractal_EDA_Preboarding/blob/main/nyc_taxi_trip_duration.csv)). The analysis was performed in Python using a Jupyter Notebook and includes comprehensive visualizations, feature engineering, and insights that could assist in downstream tasks such as machine learning model building or business analysis.

---

## 📁 Files in this Repository

- `EDA.ipynb` – Jupyter Notebook containing step-by-step EDA with explanations and visualizations.
- `nyc_taxi_trip_duration.csv` – Raw dataset used for the analysis.

---

## 🧰 Tools and Libraries Used

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- datetime
- folium (for geospatial visualizations)
- sklearn (for feature scaling and analysis)

---

## 🚶‍♂️ Step-by-Step Analysis

### 1. 📥 Data Import and Overview
- Loaded `nyc_taxi_trip_duration.csv` using pandas.
- Previewed the dataset with `.head()`, `.info()`, and `.describe()`.
- Identified key columns such as `pickup_datetime`, `dropoff_datetime`, `passenger_count`, `trip_duration`, and coordinates.

### 2. 🧹 Data Cleaning
- Checked for nulls and missing values.
- Removed outliers based on unrealistic values (e.g., trip_duration < 60 seconds or > 2 hours).
- Converted datetime columns to appropriate `datetime` objects.

### 3. 📊 Univariate and Bivariate Analysis
- **Trip Duration Distribution**: Log-transformed the target variable for better visualization.
- **Passenger Count Analysis**: Identified common passenger counts (e.g., solo vs group trips).
- **Vendor ID and Store-and-Forward Flag**: Analyzed categorical fields.

### 4. 📆 Temporal Features Engineering
- Extracted date-related features such as:
  - Hour of the day
  - Day of the week
  - Month
  - Weekday/weekend classification
- Visualized trip trends over hours and days.

### 5. 📍 Geospatial Analysis
- Plotted pickup and dropoff locations using:
  - Scatter plots for general distribution
  - Folium for interactive maps
- Analyzed trip clusters around key NYC landmarks.

### 6. 🧮 Distance Features
- Calculated **Haversine distance** between pickup and dropoff coordinates.
- Derived average speed = distance / time and visualized abnormal patterns.

### 7. 🔍 Correlation and Heatmap
- Examined feature correlations using heatmaps.
- Investigated multicollinearity and relationships with the target variable.

---

## 📈 Key Insights

- Most trips occur between 4–6 PM on weekdays.
- Trips with more than 4 passengers are rare.
- Vendor 2 tends to report shorter average trip durations.
- Outliers such as extremely long/short durations and zero distances were found and addressed.

---

## 🚀 Future Work

- Model building for predicting trip duration using engineered features.
- Clustering frequent pickup/dropoff locations.
- Adding external features like weather and traffic data.

---

## 📌 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/nyc-taxi-eda.git
   cd nyc-taxi-eda

2. Launch the Jupyter Notebook:

   ```bash
   jupyter notebook EDA.ipynb
   ```


## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.


## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.


## 📬 Contact

For questions or collaborations, reach out at \[[akshaygrandhi123@gmail.com](mailto:akshaygrandhi123@gmail.com)].

