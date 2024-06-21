Solar Wind Prediction Project
This project aims to predict the Kp-index (a measure of geomagnetic activity) using a neural network model and solar wind data. The Kp-index is crucial for understanding and forecasting space weather events that can impact Earth's communication systems, power grids, and satellites.

Project Structure
_data/omni_csvs/DatedFullData.csv: The raw dataset containing solar wind parameters and the Kp-index.
solar_wind_prediction.ipynb: Jupyter Notebook containing the data preprocessing, model building, training, and evaluation code. (You can convert this to a .py file if desired).
solar_wind.h5: The saved Keras model file (if you decide to save it).
README.md: This file, providing project details.
Dependencies
Python 3.x
NumPy
pandas
matplotlib
seaborn
TensorFlow
Keras
scikit-learn
Installation
Clone this repository: git clone [your-repository-url]
Install the required packages: pip install -r requirements.txt (Create a requirements.txt file listing the dependencies)
Data
The dataset used in this project is "DatedFullData.csv," which contains solar wind parameters such as:

Rot#: Bartels rotation number
ABS_B: Absolute value of the interplanetary magnetic field (IMF)
T: Proton temperature
V: Solar wind speed
Pressure: Solar wind dynamic pressure
R: Sunspot number
F10_INDEX: Solar radio flux at 10.7 cm
DST: Disturbance storm time index
AP_INDEX: Planetary geomagnetic activity index
AL_INDEX: Auroral electrojet index
PC_N_INDEX: Polar cap north index
Solar_Lyman_alpha: Solar Lyman-alpha emission
KP: Kp-index (target variable)
Methodology
Data Loading and Preprocessing:

Load the dataset from DatedFullData.csv.
Set the Datetime column as the index.
Drop irrelevant columns based on correlation analysis.
Split the data into training, validation, and testing sets.
Standardize the features.
Model Building:

Create a sequential neural network with two hidden layers (64 neurons each) using ReLU activation.
Use linear activation for the output layer (Kp-index is continuous).
Apply L2 regularization to the bias of the second hidden layer to prevent overfitting.
Model Training:

Compile the model with mean squared error loss and the Adam optimizer.
Train the model for 70 epochs with a batch size of 256.
Validate during training to monitor performance on unseen data.
Model Evaluation:

Calculate RMSE and R-squared on the test set.
Visualize the actual vs. predicted Kp-index values.
Results
RMSE: 0.7544 (lower is better, indicates how far off predictions are on average)
R-squared: 0.9963 (high value indicates the model explains a large portion of the variance in the target variable)
The model's high R-squared suggests strong predictive power.
