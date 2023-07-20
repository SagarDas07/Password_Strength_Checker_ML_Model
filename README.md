# SecurePassword - Password Strength Prediction Model

This Jupyter Notebook contains the code for a Password Strength Prediction Model using machine learning. The model is trained to predict the strength of a password as either "Weak," "Medium," or "Strong" based on a given dataset of passwords and their corresponding strength labels.

### Dataset

The dataset used in this project is stored in the CSV file `passwordData.csv`. It contains two columns - "password" and "strength." The "password" column contains different passwords, and the "strength" column contains numeric labels (0, 1, or 2), which correspond to "Weak," "Medium," and "Strong" password strengths, respectively.

### Dependencies

To run this notebook, you need the following dependencies installed:

- pandas
- numpy
- scikit-learn

You can install these dependencies using `pip`

```bash
pip install pandas numpy scikit-learn
```

### How to Use the Notebook

1. Load and Inspect the Dataset

- The notebook begins by loading the dataset from `passwordData.csv`.
- It displays the first few rows of the dataset to give an overview of the data.

2. Data Preprocessing

- Check for any missing values in the dataset.
- Drop rows with missing values, if any.

3. Convert Strength Labels

- Map the numeric strength labels to meaningful text labels ("Weak," "Medium," "Strong").

4. Tokenize and Split Data

- Define a function to tokenize the passwords and convert them into numerical vectors using the TF-IDF vectorizer.
- Split the data into training and testing sets.

5. Train the Model

- Create a RandomForestClassifier and train it on the training data.

6. Evaluate the Model

- Make predictions on the test data and display the predicted strengths.

7. Model Accuracy

- Calculate and print the accuracy of the model on the test data.

8. Predict Password Strength

- Input a password and predict its strength using the trained model.

### How to Run the Notebook

1. Ensure you have the required dataset named `passwordData.csv` in the same directory as the notebook.
2. Install the necessary dependencies as mentioned in the "Dependencies" section.
3. Run each cell sequentially to execute the code and observe the results.

### Sample Output

- After running cell 13, you should see the model's accuracy on the test data, which will be approximately 95.23%.
- When you run cell 14, you will be prompted to enter a password. Upon providing the password, the model will predict its strength and display the output.

### Note

This notebook assumes that the dataset `passwordData.csv` is correctly formatted with columns "password" and "strength." If you encounter any issues, make sure the dataset is appropriately structured and located in the same directory as the notebook.
