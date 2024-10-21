# Assignment 1: Laptop Price and Condition Prediction

**Dataset**: Laptop specifications from eBay.

**Tasks**:
- Implement Decision Tree and Random Forest classifiers and regressors.
- Predict laptop condition and price using the specified features.
- Perform data visualization and preprocessing.
- Compare custom implementations with sklearn's built-in models.

### Data

In this exercise, you will be working with a dataset containing information about various laptops listed on eBay. The dataset includes details on the brand, specifications, condition, and price of each laptop. The data has 2,939 entries divided into 10 columns.

#### Variables

| Column             | Description                                                        |
|--------------------|--------------------------------------------------------------------|
| Brand              | The manufacturer of the laptop.                                    |
| Product_Description| A raw description of the laptop, extracted from eBay.              |
| Screen_Size        | The diagonal size of the laptop's display, measured in inches.     |
| RAM                | The amount of Random Access Memory (RAM) in gigabytes (GB).        |
| Processor          | The type and generation of the laptop's central processing unit (CPU). |
| GPU                | The graphics processing unit (GPU) present in the laptop.          |
| GPU_Type           | Indicates whether the GPU is integrated or dedicated.             |
| Resolution         | The display resolution of the laptop screen in 'width x height'.   |
| Condition          | The physical and operational state of the laptop (New, Refurbished, etc.). |
| Price              | The cost of the laptop in USD.                                     |

#### Data Split
- **Training set**: rows 0 to 2,057 (inclusive).
- **Validation set**: rows 2,058 to 2,498 (inclusive).
- **Test set**: rows 2,499 to 2,938 (inclusive).

---

### Requirements

#### Section A 

1. **Decision Tree**
    - Implement a Decision Tree classifier and regressor algorithm in Python.

2. **Random Forest**
    - Implement a Random Forest classifier and regression algorithm in Python. For the regressor, at test time, implement average.

    - For all implementations include hyperparameter tuning for at least one parameter.

#### Section B 

1. **Data Visualization**
    - Explore the data using visualizations. The goal of this section is to get insights on the data which may or may not be relevant for the following sections.
    
    - Plots should have an informative main title, axis labels, and a legend. For each plot, provide a short description of key observations. You are required to have a minimum of three plots.

2. **Data Prep**
    - Some features have missing values, handle them accordingly and explain your choice of dealing with them.

---

#### Section C 

1. **Classification**
    - Use both models from Section A and predict the laptop condition as one of two options:
        1. 'New' which includes the categories 'New' and 'Open Box'.
        2. 'Refurbished' which includes 'Excellent - Refurbished', 'Very Good - Refurbished', and 'Good - Refurbished'.

    - Features to use: Brand, Screen_Size, RAM, Processor, GPU, GPU_Type, Resolution, Price.

2. **Regression**
    - Use both models from Section A and predict the laptop price using the following features:
        Brand, Screen_Size, RAM, Processor, GPU, GPU_Type, Resolution, Condition.

---

#### Section D 

1. **Sklearn Models**
    - Implement the models from Section C (including hyperparameter tuning) using the built-in functions from the sklearn library.

2. **Comparison**
    - Compare the results of your program and the built-in sklearn models in terms of metrics and runtime. If there are large differences, suggest an explanation as to why.
    
    - Compare the results of the Random Forest regressor when using average and median at test time. Comment on the differences.

---

#### Section E 
1. **Screen Resolution**
    - Split the Resolution column into two different numerical columns of height and width, implement both the classification and regression tasks again using your models and compare the results to Section B results. Discuss the changes.

2. **Classification Metric**
    - Report the sensitivity and specificity metric of Section C. Is there a significant difference between the scores? Suggest an explanation as to why this may be the case. Suggest a method to improve the score.

3. **Random Forest Regression Test**
    - Change your implementation of testing the random forest regression to median (Section A), rerun the implementation in Section C. Compare the new results with using the average. Discuss the changes and reflect on them.

