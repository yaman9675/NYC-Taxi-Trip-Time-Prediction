# NYC Taxi Trip Prediction
# Problem Description
Task is to build a model that predicts the total ride duration of taxi trips in New York City. Primary dataset is one released by the NYC Taxi and Limousine Commission, which includes pickup time, geo-coordinates, number of passengers, and several other variables.

<h2> :floppy_disk: Project Files Description</h2>

<p>This repository includes 1 colab notebook (.ipynb) file and 1 pdf file of project presentation. </p>
<h4>About Files:</h4>
<ul>
<li><b>NYC Taxi Trip Time Prediction Capstone Project.ipynb</b> - This file includes Features description, exploratory data Analysis, feature engineering, feature scaling and implemented algorithms for eg. <b>Linear Regression, Decision Tree, XGBoost.</b></li> 
 <li><b>NYC_PPT</b> -  This is a power point presentation file of a project. It includes various visualaized plots of EDA using <b>Seaborn and Matplotlib</b>. The result chart of various implemented algorithms.</li>
  

![---------------------------------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h2> :clipboard: Summary</h2>
<p align="justify">The given dataset conatins more than 14 lac records and 11 columns. The main goal of this project to predict the trip duration. To get more insights about the dataset, performed Exploratory data analysis to understand the main characteristics of various features. Using existing features, created new features for model building and to interpret data more easily. After analyzing the dataset, it’s found that there is a some inconsistency in some recorded data. The passenger count was high like 7 to 9 passengers in taxi. The travelled distance is very less but trip duration is quite high. There were many outliers in many columns and after analyzing the data, those outliers removed and dataset prepared for model building. Various algorithms apllied on prepared dataset afetr train and test split of dataset. <b>Linear Regression algorithm performed very poorly on given dataset. It predicted 0.60 R2 score on train and test dataset. Decision Tree predicted 0.99 for Train dataset and 0.49 for test. It’s observed that its a overfitting model. XG Boost predicted good accuracy on train and test dataset. It predicted 0.77 and 0.76 R2 score.<b/></p>

![---------------------------------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<!-- CREDITS -->
<h2 id="credits"> :scroll: Credits</h2>

<b>Yaman Saini</b> | Avid Reader | Data Science enthusiast |

[![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yamansaini14/)
[![Medium Badge](https://img.shields.io/badge/Medium-1DA1F2?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@ys726507)


![---------------------------------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
<h2>Algorithm References:</h2>
<ul>
  <li><p>Linear Regression</p>
      <p>Link: https://towardsdatascience.com/linear-regression-using-python-b136c91bf0a2</p>
  </li>
  <li><p>Decision Tree</p>
      <p>Link: https://towardsdatascience.com/the-complete-guide-to-decision-trees-28a4e3c7be14</p>
  </li>
  <li><p>XG Boost</p>
      <p>Link: https://towardsdatascience.com/a-journey-through-xgboost-milestone-3-a5569c72d72b</p>
  </li>
  <li><p>Random Forest</p>
      <p>Link: https://www.analyticsvidhya.com/blog/2021/10/an-introduction-to-random-forest-algorithm-for-beginners/</p>
  </li>
 <li><p>Hyperparameter Tuning</p>
      <p>Link: https://towardsdatascience.com/how-to-tune-a-decision-tree-f03721801680</p>
  </li>
</ul>
 
 <h2>Data Source</h2>
  <li><p>Kaggle</p>
      <p>Link: https://www.kaggle.com/c/nyc-taxi-trip-duration</p>

![---------------------------------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
