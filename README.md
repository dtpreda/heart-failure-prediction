# heart-failure-prediction

This is a simple project to predict heart failure using a dataset from Kaggle. The dataset can be found [here](https://www.kaggle.com/andrewmvd/heart-failure-clinical-data).

## Data Analysis

I did the data analysis following [this tutorial](https://www.kaggle.com/code/durgancegaur/a-guide-to-any-classification-problem/notebook), as a way to practice general data science skills.

However, I took some different decisions as well, such as replacing 0 values in the `cholesterol` column with the median value, which wasn't done in the tutorial. Be sure to check the notebook for more details.

## Model

I used this project as a way to practice with Keras, so I decided to use a simple neural network with a few layers. I used ELU as the activation function for the hidden layers, and sigmoid for the output layer. I also used the Nadam optimizer, which demonstrated to be more stable than Adam for this problem.

For regularization, I used dropout layers, with different dropout rates for each layer.

The loss function used was binary crossentropy, and the metric was accuracy.

## Results

The loss function used was binary crossentropy, and the metric was accuracy.

| Model | Accuracy | Loss |
| --- | --- | --- |
| Baseline | 0.8913 | 0.2912 |