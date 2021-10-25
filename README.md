# Neural_Network_Charity_Analysis
## Overview

The purpose of this project was to utilize deep learning through tensor flow, to create neural networks in order to analyze the alphabet soup charities donations success. We did this by pre-processing compiling training and optimizing the model to try to create the most accurate Machine learning model we could. We had a target accuracy of above 75% and created three separate optimization strategies for that. 

## Results

### Data Preprocessing

- For all three models, our target was considered the is_successful column, as that was the end result we were trying to predict through our neural network.

- For models one and three our features were application type, affiliation, classification, use case, organization, status, income AMT, special considerations, and ask AMT, for the second model we removed use case and special considerations in order to try to provide less variables to confuse our network.

- As stated before hand, and model two we removed use case and special considerations, however all three models also removed EIN and name. These are just labels or non-substantial data points that could just add more confusion to our model.

![image](url:)

### Compiling, Training, and evaluating the model

- For model one, I decided to create for hidden layers, with the first layer having 150 neurons, the second layer having 100 neurons, the third layer having 50 neurons, and the fourth layer having 25 neurons. I believed increasing the amount of neurons in my model, which I did across-the-board for all of my optimizations. The first optimization attempt also had two different activation functions. The first three layers had a tanh function. And the output layer had a sigmoid activation function. I’d be able to create a more accurate result by utilizing the neurons to handle the large amount of information that it needed to process more effectively. In through using different activation functions I thought that would classify the data in a more accurate way since tanh better represents a logistics sigmoid, which would help us better classify our binary target result of successful or not.

![image](url:)
![image](url:)

- The second model had only two hidden layers with 80 neurons than 40 neurons, are used a RELU and then sigmoid activation function. I also changed the replace value counts to 200 from 600 in the last model. I was trying to see if having less replacements and following a higher neuron, but more closely related to our standard approach for neural networks would remove some errors that would be created from the first model by having too many neurons through overfitting.

![image](url:)
![image](url:)

- The third optimization brought the replace lists up to replace if <1000. And we ran a simulation similar to the first neural net work but with3  hidden layers that were all tanh activation functions except the last sigmoid function. However I drop the neurons down to 100, 80, and 30. I didn’t see the results I was looking for and the second optimization compared to the first one. Once again worrying about overfitting, I thought that this would produce the best result.

![image](url:)
![image](url:)

- All three of the simulations failed to break the 75% model accuracy target, however I did see some epochs reach into the low 74% accuracy‘s so I know I was getting there. This is very disappointing and I believe I would need more time to make this model more accurate.

 - The main steps I took to increase model performance was trying to increase the amount of layers and neurons I could play with, playing around with the activation functions, and modifying the value count replacements that are earlier in the model. these are the three optimizations that I got the most decent results with however there were more attempts than just three. However I believe that the data was getting there.

## Summary

Overall, we were able to push the models accuracy up slightly by pulling around with all of the different components that we mentioned above in the results, However, ultimately we were unsuccessful. If I were to do this again with a separate machine learning format I would probably do a decision trees approach through random forest classifier to see what a classified output will look like in comparison to a deep neural network model especially since we’re going for a more binary target with the is successful column.

