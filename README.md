Solar Wind AI Project
This project is focused on predicting solar wind conditions using machine learning techniques. The goal is to develop a model that can accurately forecast the solar wind parameters based on historical data.

Data
The data used for this project is sourced from the NASA space apps program. It includes a dataset containing various solar wind features such as IMF (Interplanetary Magnetic Field), PLS (Plasma Sheet), ABS_B (Absolute B), and many others. The dataset also includes the target variable, which is the KP index, used as a measure of the Earth's geomagnetic activity.

Dependencies
The project relies on the following libraries and frameworks:

Numpy
Pandas
Matplotlib
Seaborn
TensorFlow
Keras
Scikit-learn
Make sure to have these dependencies installed in your Python environment before running the code.

Usage
Download the dataset file (DatedFullData.csv) from the specified location.
Update the file path in the code to match the location where you saved the dataset.
Run the code to load the data, preprocess it, and train the machine learning model.
The model will be saved after training, and you can use it for making predictions on new data.
Model Evaluation
The project includes various evaluation metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared (R2) score. These metrics provide insights into the performance of the model in predicting the KP index.

Additional Information
For more details about the project and the code implementation, please refer to the Jupyter Notebook file (solar_wind.ipynb) provided in this repository.

Conclusion
The Solar Wind AI Project aims to develop an accurate predictive model for solar wind conditions. By leveraging machine learning techniques and historical data, we can gain valuable insights into the behavior of the solar wind and its impact on Earth's geomagnetic activity.
