# Password Strength Checker

This project is a password strength checker that uses a Random Forest classifier to predict the strength of passwords based on their characteristics. It leverages machine learning techniques to classify passwords into three categories: Weak, Medium, and Strong.

## Prerequisites

Make sure you have Python installed on your system. Additionally, install the required libraries listed in `requirements.txt` using the following command:

```bash
pip install -r requirements.txt
```

## Features

- Reads password data from a CSV file (`data.csv`).
- Utilizes TF-IDF vectorization to convert password strings into numerical features.
- Implements a Random Forest classifier for password strength prediction.
- Provides a command-line interface for users to input passwords and check their strength.

## Usage

1. Clone or download the project files to your local machine.

2. Ensure you have a dataset named `data.csv` containing password data with corresponding strength labels (0 for Weak, 1 for Medium, and 2 for Strong).

3. Run the Python script `main.py` in your terminal or preferred Python environment.

4. Follow the prompts to enter a password for strength evaluation. The program will output the predicted strength category (Weak, Medium, or Strong) for the entered password.

## File Structure

- `main.py`: Contains the main script for password strength checking.
- `data.csv`: CSV file containing password data and strength labels.
- `requirements.txt`: Lists the required Python libraries and versions.

## How it Works

1. The script loads the password dataset from `data.csv` and preprocesses the data by handling missing values and mapping strength labels.

2. Password strings are tokenized and converted into numerical features using TF-IDF vectorization (`TfidfVectorizer`).

3. The dataset is split into training and testing sets using `train_test_split` from sklearn.

4. A Random Forest classifier (`RandomForestClassifier`) is trained on the training data to predict password strengths.

5. Users can input a password through the command line, and the program uses the trained model to predict its strength category.

## Contributing

Contributions to this project are welcome! You can contribute by improving the model's accuracy, adding new features, enhancing the user interface, or fixing bugs. Fork the repository, make your changes, and submit a pull request with a detailed description of your modifications.
