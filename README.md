# Glass Project

The goal of this project is to perform the classification of glass materials based on their chemical composition.
This dataset was download from the Kaggle website: https://www.kaggle.com/datasets/uciml/glass

Original source: https://archive.ics.uci.edu/ml/datasets/Glass+Identification


## Dataframe

This dataset is quite small. As we can observe, only 214 obervations and 10 variables are at our disposal. 

![image](https://user-images.githubusercontent.com/67120829/184669689-7d85f644-1745-4d5c-a40a-471f3e11b274.png)

There is 9 predictive variables (features) and 1 target variable. 
#### Predictive variables
- RI: Refraction index of the glass.
- Na, Mg, Al, Si, K, Ca, Ba, Fe: weight percent in corresponding oxide used to synthetize the glass.

#### Target variable
- Type: the type of glass which can be one of 6 categories represented by an integer in the dataset (correspondance below).
 
1: Building Window (processed)

2: Building Window (non processed)

3: Vehicule Window (processed)

5: Container

6: Tableware

7: Headlamp


### Data Analysis

##### Data types and Missing values

The variables are of two types: float (continues values) and integer (discrete values) and no values are missing.

![image](https://user-images.githubusercontent.com/67120829/184670449-f169c954-bd4a-431a-8ba2-9b4749a070f1.png)

##### Data statistical description

Some of the variables are skew (Mg) and others are well centered (Si). Indeed, the mean and the median of the Mg variable are quite different and very similar for the Si variable. Also, the standard deviations of th eMg variable is high and low for the Si variable.

![image](https://user-images.githubusercontent.com/67120829/184683064-4d68f7ec-eacd-43d2-beb2-c3fb63dca428.png)

We can add that the variables don't have the same scale.

- We can observe that the weighted percentage of the Si oxyde is way higher than the other oxyde. This is explained by the fact that glass are mostly made of Si oxyde.

#### Data correlation

The analysis of the data correlation is a good way to detect redundant features that can be discard. In our case, we looked at correlation between features only (the target variable is categorical).

The next figure report the absolute value of the spearman correlation for each variable with the other.

![image](https://user-images.githubusercontent.com/67120829/184677530-9fae211e-33d0-41a4-b281-e19dc7d3d897.png)

The most correlated variables are the Ca oxyde and the reflective index (0.7). We can assume that modifying Ca oxyde can have an important impact on the reflective index of the glass.
The features are not sufficiently correlated to be discard so we keep them all.

#### Target modes

As mentioned before, there is 6 categories of glass in the target variable. The graphique below displays the proportion of each categories.

![image](https://user-images.githubusercontent.com/67120829/184688350-f445c7e6-bb66-4204-89a0-aa50f90c5fd2.png)

AS we can observe, the categories are highly unbalanced with 36% of the data belonging to the "Building Window (processed)" category and 4% of the data belonging to the "Headlamp" category.








