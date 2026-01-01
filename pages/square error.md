- sum of the squares of these distances #card
  card-last-interval:: 4
  card-repeats:: 1
  card-ease-factor:: 2.6
  card-next-schedule:: 2026-01-05T18:52:37.688Z
  card-last-reviewed:: 2026-01-01T18:52:37.688Z
  card-last-score:: 5
- ![image.png](../assets/image_1767178417793_0.png)
- the square error is used more commonly in practice than the absolute error. Why? A square has a much nicer derivative than an absolute value, which comes in handy during the training process.
- the **mean square error** is the average of the squares of these same distances #card
- **root mean square error**. It is used to match the units in the problem and also to give us a better idea of how much error the model makes in a prediction. How so? Imagine the following scenario: if we are trying to predict house prices, then the units of the price and the predicted price are, for example, dollars ($). The units of the square error and the mean square error are dollars squared, which is not a common unit. If we take the square root, then not only do we get the correct unit, but we also get a more accurate idea of roughly by how many dollars the model is off per house. #card
- **dot product** To code the RMSE function, we used the dot product, which is an easy way to write a sum of products of corresponding terms in two vectors.