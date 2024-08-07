# Digit Recognition Project

This project is a digit recognition system implemented in Python using a neural network built from scratch without using popular libraries such as TensorFlow. The system is trained on a dataset of handwritten digits and can predict the digit in a new image.

## Project Structure

The project is structured as follows:
```
digit_reco/
    digit_reco.ipynb
    digit-recognizer/
        sample_submission.csv
        test.csv
        train.csv
README.md
```

The main code is in the Jupyter notebook `digit_reco.ipynb`. The `digit-recognizer` directory contains the data used for training and testing the neural network.

## How to Use

1. Open the `digit_reco.ipynb` file in a Jupyter notebook environment.
   
2. Run the cells in order to load the necessary libraries, load the data, train the neural network, and make predictions.
   
3. The data is loaded from the `train.csv` and `test.csv` files in the `digit-recognizer` directory. The `train.csv` file is used to train the   neural network and the `test.csv` file is used to test the network's predictions. Due to GitHub policies the dataset can't be store, to download it enter the following command in a terminal :
   `kaggle competitions download -c digit-recognizer`
   
4. The neural network is trained using the `gradient_descent` or `gradient_descent_adam` functions. These functions take the training data and some parameters for the gradient descent algorithm and return the weights and biases of the trained network.

5. After training the network, you can use the `make_predictions` function to make predictions on new data. This function takes the weights and biases of the network and some input data and returns the network's predictions.

6. The predictions are then compared to the actual labels in the `test_prediction`. We use the `test_prediction_test` to test on the test dataset.

## Dependencies

This project requires the following Python libraries:
- numpy
- pandas
- matplotlib

## Data

The data used in this project is from the Kaggle Digit Recognizer competition. The data consists of 28x28 pixel images of handwritten digits. The `train.csv` file contains 42,000 images and the `test.csv` file contains 28,000 images. Each image is labeled with the correct digit (0-9).
