
![Logo](https://github.com/swarnadeep13/California-Housing-Dataset-Linear-regressor/blob/main/houses.png)


# Project Title

Linear regression model in California Housing data


## Implementation Details

- Dataset: California Housing Dataset ([view below for more details](https://www.kaggle.com/datasets/camnugent/california-housing-prices))
- Model: [Linear Regressor](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
- Input: 8 features - Median Houshold income, House Area, ...
- Output: R2 and MSE for various models in a quest to search for "Good" Models

## Dataset Details

This dataset was obtained from the StatLib repository ([Link](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html))

This dataset was derived from the 1990 U.S. census, using one row per census block group. A block group is the smallest geographical unit for which the U.S. Census Bureau publishes sample data (a block group typically has a population of 600 to 3,000 people).

A household is a group of people residing within a home. Since the average number of rooms and bedrooms in this dataset are provided per household, these columns may take surprisingly large values for block groups with few households and many empty houses, such as vacation resorts.

It can be downloaded/loaded using the sklearn.datasets.fetch_california_housing function.

- [California Housing Dataset in Sklearn Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)
- 20640 samples
- 8 Input Features: 
    - MedInc median income in block group
    - HouseAge median house age in block group
    - AveRooms average number of rooms per household
    - AveBedrms average number of bedrooms per household
    - Population block group population
    - AveOccup average number of household members
    - Latitude block group latitude
    - Longitude block group longitude
- Target: Median house value for California districts, expressed in hundreds of thousands of dollars ($100,000)

## Evaluation and Results

LinearRegression

| Metric        | Value (Training) | Value (Validation) |
| ------------- | ---------------- | ------------------ |
| R2 Score      |                  1                    |
| MSE           | 3.50e-15         | 3.39e-15           |

KNN

| Metric        | Value (Training) | Value (Validation) |
| ------------- | ---------------- | ------------------ |
| R2 Score      |                 0.034                 |
| MSE           | 0.29             | 0.33               |

RandomForestRegressor

| Metric        | Value (Training) | Value (Validation) |
| ------------- | ---------------- | ------------------ |
| R2 Score      |                 0.99                  |
| MSE           | 0.003            | 0.005              |

GradientBoostingRegressor

| Metric        | Value (Training) | Value (Validation) |
| ------------- | ---------------- | ------------------ |
| R2 Score      |                 0.99                  |
| MSE           | 0.006            | 0.006              |


Ensemble learning techniques the Mean Squared error has significantly come down and had a positive impact on the model buidling

## Key Takeaways

What did you learn while building this project? What challenges did you face and how did you overcome them?


## How to Run

The code is built on Google Colab on an iPython Notebook. 

```bash
Simply download the repository, upload the notebook and dataset on colab, and hit play!
```


## Roadmap

What are the future modification you plan on making to this project?

- Try more models

- Wrapped Based Feature Selection


## Libraries 

**Language:** Python

**Packages:** Sklearn, Matplotlib, Pandas, Seaborn



## Acknowledgements

All the links, blogs, videos, papers you referred to/took inspiration from for building this project. 

 - [Awesome Example](https://medium.com/@basumatary18/implementing-linear-regression-on-california-housing-dataset-378e14e421b7)
 - [Awesome README](https://readme.so/)



## Contact

If you have any feedback/are interested in collaborating, please reach out to me at swarnadeep.mandal@gmail.com


## License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

