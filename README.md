
# Hotel Room Price Prediction for Booking.com

## Introduction
This project aims to predict hotel room prices based on the following factors:
- Hotel location
- Hotel type
- Room area
- Rating
- Number of reviews
- Distance from city center

The machine learning algorithms used include:
- **K-Nearest Neighbors (KNN)**
- **Linear Regression**
- **Random Forest**

The dataset is collected and processed from [Booking.com](https://www.booking.com/).

## Technologies and Libraries
- **Python**: Main programming language
- **Key Libraries**:
  - `BeautifulSoup`: Web scraping from HTML
  - `pandas`, `numpy`: Data manipulation
  - `sklearn`: Building machine learning models
  - `matplotlib`, `seaborn`: Data visualization

## Steps
1. **Data Collection**:
   - Crawl data from Booking.com using `BeautifulSoup`.
   - Save raw data to `rawdata.csv`.
2. **Data Processing**:
   - Clean data, handle missing values and outliers.
   - Normalize data using Min-Max Scaling.
   - Encode categorical data with `LabelEncoder`.
3. **Modeling**:
   - Test algorithms KNN, Linear Regression, and Random Forest.
   - Compare model performance using metrics: RMSE, MAE, and Variance.
   - Select Random Forest with an accuracy of 81%.
4. **Model Optimization**:
   - Hyperparameter tuning with GridSearchCV.
   - Feature selection based on importance (e.g., `type_hotel`, `area`, `rating`).

## Results
- Achieved **81% accuracy** in predicting room prices using the Random Forest model.
- Improved results by 4-6% through hyperparameter tuning and feature selection.

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Collect data:
   - Run the `crawlbookings.py` file:
     ```bash
     python crawlbookings.py
     ```
4. Run the main script:
   ```bash
   python main.py
   ```

## Future Development
- Collect additional data to enhance prediction accuracy.
- Explore advanced algorithms like XGBoost or Neural Networks.
- Apply alternative Feature Engineering techniques such as OneHotEncode.

## References
1. [Linear Regression](https://dominhhai.github.io/vi/2017/12/ml-linear-regression/)
2. [KNN Algorithm](https://codelearn.io/sharing/thuat-toan-k-nearest-neighbors-knn)
3. [Random Forest](https://machinelearningcoban.com/tabml_book/ch_model/random_forest.html)
