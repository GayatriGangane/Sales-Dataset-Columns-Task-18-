# Dataset Column Selection Using Pandas

## Project Overview

This project demonstrates how to load and work with the **Iris dataset** using Python and Pandas. It focuses on selecting rows and columns using Pandas `loc` and `iloc`, along with conditional data selection.

The project is implemented in a **Jupyter Notebook**.

## Objectives

* Load the Iris dataset using Scikit-learn.
* Convert the dataset into a Pandas DataFrame.
* Display dataset information and column names.
* Select columns using `loc`.
* Select columns using `iloc`.
* Select rows using `loc`.
* Select rows using `iloc`.
* Select specific rows and columns.
* Perform conditional selection.
* Perform selection using multiple conditions.
* Display basic dataset statistics and class distribution.

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

## Dataset

The project uses the **Iris dataset**, which contains measurements of iris flowers.

### Features

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

### Target Classes

* Setosa
* Versicolor
* Virginica

The dataset contains **150 records and 5 original attributes**, with additional target and target-name columns added during preprocessing.

## Pandas Selection Methods

### 1. `loc`

The `loc` method is used for label-based selection of rows and columns.

Example:

```python
df.loc[:, ["sepal length (cm)", "sepal width (cm)", "target_name"]]
```

### 2. `iloc`

The `iloc` method is used for position-based selection of rows and columns.

Example:

```python
df.iloc[:, [0, 1, 4, 5]]
```

### 3. Conditional Selection

Conditions can be used to filter records.

Example:

```python
df[df["sepal length (cm)"] > 6.0]
```

### 4. Multiple Conditions

Multiple conditions can be combined using logical operators.

Example:

```python
df[
    (df["sepal length (cm)"] > 6.0) &
    (df["petal length (cm)"] > 4.0)
]
```

## Project Workflow

1. Import required libraries.
2. Load the Iris dataset.
3. Convert the dataset into a DataFrame.
4. Add target labels.
5. Display rows and columns.
6. Demonstrate `loc` selection.
7. Demonstrate `iloc` selection.
8. Apply conditional filtering.
9. Apply multiple conditions.
10. Display dataset statistics and class distribution.

## How to Run

### Step 1: Install Required Libraries

```bash
pip install pandas numpy scikit-learn jupyter
```

### Step 2: Start Jupyter Notebook

```bash
jupyter notebook
```

### Step 3: Create a Notebook

Create a new Python notebook and paste the provided project code.

### Step 4: Run the Cells

Run the notebook cells sequentially to view the dataset selections and results.

## Expected Output

The notebook displays:

* Dataset shape
* Column names
* First 10 records
* Columns selected using `loc`
* Columns selected using `iloc`
* Rows selected using `loc`
* Rows selected using `iloc`
* Specific row and column selections
* Records satisfying conditions
* Records satisfying multiple conditions
* Dataset summary statistics
* Target class distribution

## Conclusion

This project provides practical knowledge of **Pandas DataFrame indexing and filtering**. It demonstrates the difference between label-based selection using `loc` and position-based selection using `iloc`. Conditional selection is also demonstrated for extracting meaningful records from a dataset.

## Author

**Gayatri Dipakrao Gangane**

