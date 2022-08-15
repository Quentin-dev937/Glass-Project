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
- Na, Mg, Al, Si, K, Ca, Ba, Fe: weight percent in corresponding oxide.

#### Target variable
- Type: the type of glass which can be one of 6 categories represented by an index (correspondance below).
 
1: "Building Window (processed)"

2: "Building Window (non processed)"

3: "Vehicule Window (processed)"

5: "Container"

6: "Tableware"

7: "Headlamp"


### Data Analysis

![image](https://user-images.githubusercontent.com/67120829/184670449-f169c954-bd4a-431a-8ba2-9b4749a070f1.png)

The variables are of two types: float (continues values) and integer (discrete values) and no values are missing.


![image](https://user-images.githubusercontent.com/67120829/184683064-4d68f7ec-eacd-43d2-beb2-c3fb63dca428.png)

- the scale of the values is heterogen
- the range of the values is also very heterogen

### Data vizualisation


![image](https://user-images.githubusercontent.com/67120829/184677530-9fae211e-33d0-41a4-b281-e19dc7d3d897.png)






