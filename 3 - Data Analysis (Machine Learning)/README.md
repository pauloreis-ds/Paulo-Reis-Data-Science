# Machine Learning

Machine learning is based on the idea that systems can analyze and learn from data to then identify patterns and make decisions with minimal human intervention.

        In a simplified way:
        feature is the data we provide for a machine to learn.
        label is What we want to predict.

<p align="center">
<img  height="300" src="https://github.com/pauloreis-ds/Paulo-Reis-Ciencia-de-dados/blob/master/3%20-%20An%C3%A1lise%20de%20dados%20(com%20Machine%20Learning)%20-%20Data%20Analysis%20(Machine%20Learning)/just_images/feature_label2.png">
</p>


    The algorithm can find patterns "only" if we provide resources (information) so that it can learn.
    But after that, to tell us how the data should be classified, It also needs a set of possible classes/values/responses
    (labels) so that It knows what to do with each data that we enter. And then it knows how to classify them.

    > A feature briefly explained would be the input you have fed to the system and the label would be the output you are expecting.

    > Features are patterns, colors, forms... or so to speak, 'column names' in the training dataset. Label is the value we want to to predict.
      The output we get from our model after the training.
    
<p align="center">
<img  height="300" src="https://github.com/pauloreis-ds/Paulo-Reis-Ciencia-de-dados/blob/master/3%20-%20An%C3%A1lise%20de%20dados%20(com%20Machine%20Learning)%20-%20Data%20Analysis%20(Machine%20Learning)/just_images/feature_label.png">
</p>

Basically, the application of ML algorithms is:
      
      - Separate training data (features - X) and test (labels - y)
            - X, y - training
            - X, y - test
      - Create the model
            - Choose the most suitable.
            - Create the object() of the model, so we can access its methods.
            - Pass the training data to it.
            - Make predictions with the test data.
            - Check the accuracy of the model by comparing the test data with the responses provided by the algorithm.
      

(X, y) training: Runs the model.

(X, y) test: Validates the models.


The training set of features is what we provide to our model during training along with the answers. The goal is for the model to learn a mapping between the features and the target.

The testing set of features is used to evaluate the trained model. **The model is not allowed to see the answers for the testing set and must make predictions using only the features**. We know the answers for the test set so we can compare the test predictions to the answers.

<p align="center">
<img  height="300" src="https://github.com/pauloreis-ds/Paulo-Reis-Ciencia-de-dados/blob/master/3%20-%20An%C3%A1lise%20de%20dados%20(com%20Machine%20Learning)%20-%20Data%20Analysis%20(Machine%20Learning)/just_images/feature_label1.png">
</p>
