# Food Recall Classification Using Machine Learning

This is my MSc Statistics project. I used food recall records from the US FDA to study whether machine learning can predict the recall class (Class I, II or III).

## Dataset

The dataset contains details such as the product, reason for recall, recalling firm and recall dates. The target variable is `classification`.

Place `food_enforcement_dates_fixed.csv` inside the `data` folder before running the notebook. Check the dataset's original terms before sharing the CSV publicly.

## What I did

- Cleaned the data and explored recall patterns.
- Prepared text and other variables for modelling.
- Compared six machine learning model families.
- Used an event-based split to reduce data leakage.
- Evaluated the models using accuracy, macro F1 and other classification measures.
- Checked model errors and tested performance on later years.

## Models

Logistic Regression, Linear SVM, Complement Naive Bayes, Random Forest, LightGBM and a blended model.

## Results

The selected blend achieved about **76% accuracy** and **0.64 macro F1** on the held-out test data. Class III was harder to predict than the other two classes, mainly because it had fewer examples.

## Run the project

1. Install the libraries: `pip install -r requirements.txt`
2. Keep the CSV in the `data` folder.
3. Open the notebook in the `notebooks` folder.
4. Run the cells from top to bottom.

## Tools

Python, Pandas, NumPy, Scikit-learn, LightGBM, Matplotlib, Seaborn and Jupyter Notebook.

*This is an academic project. Its predictions are for analysis and learning, not a replacement for official FDA decisions.*
