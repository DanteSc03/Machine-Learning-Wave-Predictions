# AutoML Regression: Predicting Wave Heights 🌊

## 🚀 Overview
This project demonstrates how to use **BigQuery AutoML** to build and evaluate a regression model that predicts **significant wave height** based on oceanographic data. The pipeline includes training, evaluating, and visualizing model predictions, culminating in a scatter plot comparing actual and predicted values.

---

## 📋 Features
- **BigQuery AutoML Integration**: Leverages Google Cloud's AutoML capabilities for automated model building.
- **Model Evaluation**: Uses key metrics such as RMSE, R² score, and Mean Absolute Error (MAE) to assess performance.
- **Prediction Visualization**: Generates a scatter plot for a clear visual comparison of actual vs predicted wave heights.
- **Jupyter Notebook**: End-to-end workflow is implemented using a notebook, ensuring reproducibility and clarity.

---

## 🛠️ Tools and Libraries
- **Google BigQuery**: Data querying and AutoML model training.
- **Python**: Data processing and visualization.
- **Pandas**: For handling tabular data.
- **Matplotlib**: Creating the "Predicted vs Actual" scatter plot.

---

## 📊 Data Description
The dataset includes oceanographic features such as:
- **Significant wave height** (target variable)
- **Current speed and direction**
- **Water temperature**
- **Wind speed and wave direction**

Predictions are made on test data to evaluate model performance.

---

## 🔧 How to Run
1. **Set up Google Cloud Project**:
   - Enable **BigQuery API**.
   - Upload the training and testing data to BigQuery tables.

2. **Authentication**:
   Ensure you have set up your Google Cloud service account credentials:
   ```bash
   export GOOGLE_APPLICATION_CREDENTIALS="path/to/your/service-account.json"
   ```

3. **Run the Script**:
   Execute the Jupyter Notebook `G13.ipynb`. Key sections include:
   - Model creation using `ML.PREDICT` and `ML.EVALUATE`.
   - Saving predictions to a Pandas DataFrame.
   - Generating the scatter plot of actual vs predicted values.

4. **Install Required Libraries**:
   ```bash
   pip install google-cloud-bigquery pandas matplotlib
   ```

---

## 📈 Results
- **Model Performance Metrics**:
  - Mean Absolute Error (MAE): `0.753781`
  - Mean Squared Error (MSE): `0.798625`
  - R² Score: `0.196255` (indicating underfitting)

- **Visualization**:
  The scatter plot below shows predicted values against actual values, highlighting the underfitting issue:
  ![Predicted vs Actual](scatter_plot.png)

---

## 📝 Improvements
To address underfitting:
1. Incorporate additional features for better modeling.
2. Increase training time and data.
3. Explore more complex algorithms outside AutoML.

---

## 📂 File Structure
```
|-- G13.ipynb               # Jupyter Notebook with full pipeline
|-- scatter_plot.png        # Visualization of predictions
|-- README.md               # Project documentation
```

---

## 🎉 Acknowledgments
- **Google Cloud Platform** for AutoML capabilities.
- **Matplotlib** for visualization.
- Oceanographic data sources for providing real-world datasets.

---

## 🤝 Connect
Find me on GitHub: [DanteSc03](https://github.com/DanteSc03)

Feel free to contribute or share feedback! 🌟
