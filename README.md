
# Spam Mail Detection

This project is a machine learning-based email classification model that identifies whether an email is spam or not using the TF-IDF (Term Frequency-Inverse Document Frequency) method for feature extraction and logistic regression for classification.

## Technologies Used
- Python 3.x
- NumPy
- Pandas
- Scikit-learn

## Dataset
The dataset used for training the model contains labeled email text data. It consists of two classes: 
- **Spam**: Emails identified as spam.
- **Ham**: Non-spam emails.


## Usage

### Step 1: Prepare the Dataset
Ensure the dataset file `emails.csv` is placed in the root directory. It should contain at least two columns: one for email content and another for the spam/ham label.

### Step 2: Run the Program
Run the Python script to train and evaluate the spam detection model.

### Step 3: Results
Once the model is trained, the program will output the accuracy of the classifier on the test data. It will also provide the confusion matrix to evaluate the performance further.

## How It Works
1. **Data Preprocessing**: The email text data is preprocessed by removing any non-alphabetic characters, converting all text to lowercase, and tokenizing the text.
2. **Feature Extraction**: The TF-IDF vectorizer converts the email text into numerical feature vectors.
3. **Model Training**: A logistic regression model is trained on the feature vectors.
4. **Model Evaluation**: The model's performance is evaluated using accuracy, precision, recall, and F1 score.

## Example Output
After running the program, you will see something like this:

```
Accuracy: 97.2%
Confusion Matrix:
[[ 980   15]
 [  32  973]]
```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

