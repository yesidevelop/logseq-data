- **Basic example**
  ![image.png](../assets/image_1767168975583_0.png)
- ```Price = 100 + 50(Number of rooms)
  Price = 100 + 50(Number of rooms)
  ```
- The price per room is called the *weight* (50) of that corresponding feature, and the base price is called the *bias* (100) of the model
- **features** The features of a data point are those properties that we use to make our prediction #card
- **labels** This is the target that we try to predict from the features. In this case, the label is the price of the house. #card
- **model** A machine learning model is a rule, or a formula, which predicts a label from the features #card
- **prediction** The prediction is the output of the model. If the model says, “I think the house with four rooms is going to cost $300,” then the prediction is 300. #card
- **weights** In the formula corresponding to the model, each feature is multiplied by a corresponding factor. These factors are the weights. In the previous formula, the only feature is the number of rooms, and its corresponding weight is 50. #card
- **bias** As you can see, the formula corresponding to the model has a constant that is not attached to any of the features. This constant is called the bias. In this model, the bias is 100, and it corresponds to the base price of a house. #card
- **Complicated example**
  ![image.png](../assets/image_1767169456006_0.png)
- ![image.png](../assets/image_1767169500804_0.png)
- ```
  Price = 100 + 50(Number of rooms) + (Small error)
  ```
- **slope** The slope of a line is a measure of how steep it is. This ratio is constant over the whole line. In a machine learning model, this is the weight of the corresponding feature#card
- ***y*-intercept** The *y*-intercept of a line is the height at which the line crosses the vertical (*y-*) axis. In a machine learning model, it is the bias and tells us what the label would be in a data point where all the features are precisely zero. #card
- **linear equation** This is the equation of a line. It is given by two parameters: the slope and the *y*-intercept. If the slope is *m* and the *y*-intercept is *b*, then the equation of the line is *y* = *mx* + *b*, and the line is formed by all the points (*x,y*) that satisfy the equation #card
- ![image.png](../assets/image_1767169853770_0.png)
- **Multivariate linear regression** models the linear relationship between **multiple independent variables (predictors)** and **one or more dependent (outcome) variables** #card
- ```
  Price = 30(number of rooms) + 1.5(size) + 10(quality of the schools) – 2(age of the house) + 50
  ```
-
-
- ## How to get the computer to draw this line: The linear regression algorithm
-