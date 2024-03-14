# Sepsis Detection

This repository presents an Artificial Neural Network (ANN) model for the early prediction of sepsis from clinical data, based on the PhysioNet/Computing in Cardiology Challenge 2019 dataset.

## Dataset

The dataset consists of data and labels for 40,336 patients from hospital systems, with labels for 24,819 patients sequestered as hidden test sets. It includes a combination of hourly vital sign summaries, lab values, and static patient descriptions. The data contains 40 clinical variables, including 8 vital sign variables, 26 laboratory variables, and 6 demographic variables.

## ANN Architecture

The ANN architecture employed for sepsis detection is as follows:

- Input Layer: 19 units corresponding to the input features
- Hidden Layers:
  - Fully Connected Layer 1: 256 units, ReLU activation
  - Fully Connected Layer 2: 128 units, ReLU activation
  - Dropout Layer (25% dropout rate)
  - Fully Connected Layer 3: 64 units, ReLU activation
  - Dropout Layer (25% dropout rate)
  - Fully Connected Layer 4: 32 units, ReLU activation
  - Dropout Layer (20% dropout rate)
  - Fully Connected Layer 5: 16 units, ReLU activation
  - Dropout Layer (10% dropout rate)
- Output Layer: 1 unit with sigmoid activation, representing the probability of sepsis occurrence

## Usage

1. Clone this repository to your local machine.
2. Download the PhysioNet/Computing in Cardiology Challenge 2019 dataset from the provided link.
3. Preprocess the dataset to extract relevant features and labels.
4. Train the ANN model using the provided script or your preferred method.
5. Evaluate the trained model's performance on test data.
6. Use the trained model to predict sepsis occurrence in new patient data.


## Results

After training and evaluation, the performance metrics such as accuracy, precision, recall, and F1-score are computed and reported. Additionally, ROC curves and confusion matrices may be generated for further analysis.

## Conclusion

This project demonstrates the application of ANN models for the early detection of sepsis using clinical data. Further research and optimization can be explored to improve the model's performance and generalization capabilities.

