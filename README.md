
# Title: Credit Risk Analysis with Logistic Regression and Resampling

![Alt text](Images/12-5-challenge-image.png)

This project uses various techniques to train and evaluate machine learning models with imbalanced classes to identify the creditworthiness of borrowers. Credit risk poses a classification problem that’s inherently imbalanced, with healthy loans far outnumbering risky loans.

## Project Structure
The project includes a Jupyter notebook that uses the imbalanced-learn library and the logistic regression model to compare two versions of a dataset. The first uses the original dataset, while the second version resamples the data using the RandomOverSampler module from the imbalanced-learn library. For both cases, the notebook gets the count of the target classes, trains a logistic regression classifier, calculates the balanced accuracy score, generates a confusion matrix, and generates a classification report.

## Dataset
The dataset used for this project is read into a Pandas DataFrame from a CSV file.

## Dependencies
This project requires the following dependencies:

- Python 3.x
- Jupyter Notebook
- Pandas
- Scikit-learn
- Imbalanced-learn

## Usage
To run this project, I installed the dependencies listed above.

## Results
After splitting the data into training and testing datasets, a logistic regression model is fit using the training data. The model is then used to predict both the 0 (healthy loan) and 1 (high-risk loan) labels in the testing data. The model's performance is evaluated by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

Next, the training data is resampled using the RandomOverSampler module from the imbalanced-learn library. The logistic regression model is then fit with the resampled data, and its performance is evaluated using the same metrics as the original model.

## Summary and Analysis
Both machine learning models show good performance in terms of accuracy score, precision, and recall. However, the model trained with the resampled data performs better overall, with higher precision and recall scores for the minority class (high-risk loans).

In summary, resampling the training data with RandomOverSampler results in a logistic regression model that predicts high-risk loans with higher precision and recall, making it a better choice for identifying high-risk borrowers. Therefore, it is recommended to use the resampled data for future credit risk analysis.
Contributing
This project is open to contributions. Anyone interested can create a pull request with a clear description of the changes made.

## License
This project is licensed under the MIT License.
