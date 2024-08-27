# Solar Wind KP Index Prediction

This project aims to predict the KP index, a measure of geomagnetic activity, using solar wind data and machine learning techniques.

## Project Overview

The project uses a dataset containing various solar wind parameters and geomagnetic indices to train a neural network model for KP index prediction. The model is implemented using TensorFlow/Keras and achieves high accuracy in predicting the KP index.

## Key Features

- Data preprocessing and exploratory data analysis
- Feature selection based on correlation analysis
- Neural network model implementation using TensorFlow/Keras
- Model training and validation
- Performance evaluation using RMSE and R-squared metrics
- Visualization of training/validation loss and prediction results

## Requirements

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- TensorFlow
- Scikit-learn

## Usage

1. Ensure all required libraries are installed.
2. Load the solar wind data CSV file.
3. Run the data preprocessing steps.
4. Train the neural network model.
5. Evaluate the model performance.
6. Visualize the results.

## Model Architecture

The neural network model consists of:
- Input layer: 12 features
- Hidden layer 1: 64 neurons with ReLU activation
- Hidden layer 2: 64 neurons with ReLU activation and L2 regularization
- Output layer: 1 neuron with linear activation

## Results

The model achieves:
- RMSE: 0.7544
- R-squared: 0.9963

## Future Improvements

- Experiment with different model architectures
- Implement feature engineering techniques
- Explore other machine learning algorithms
- Incorporate real-time solar wind data for live predictions

## Contributors

[Your Name/Team Name]

## License

[Specify the license for your project]
