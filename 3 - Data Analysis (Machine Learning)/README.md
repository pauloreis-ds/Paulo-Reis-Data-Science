# Machine Learning

Machine learning is based on the idea that systems can analyze and learn from data to then identify patterns and make decisions
with minimal human intervention.

       In a simplified way:
         Feature is what we provide for the machine to "learn"/predict.
         Label is what we want to predict.

<p align="center">
<img  height="300" src="https://github.com/pauloreis-ds/Paulo-Reis-Ciencia-de-dados/blob/master/3%20-%20An%C3%A1lise%20de%20dados%20(com%20Machine%20Learning)%20-%20Data%20Analysis%20(Machine%20Learning)/just_images/feature_label2.png">
</p>


    The algorithm can find patterns "only" if we provide resources (information) so that it can learn. 
    But after that, to tell us how the data should be classified, It also needs a set of possible classes/values/responses (labels)
    so that he knows what to do with each data that we enter. So that It knows how to classify them.

    > Briefly explained, a feature would be the input data that you provided to the system and the 
      label would be the output (the answer/prediction) that is expected.

    > Features are patterns, colors, shapes ... that is, 'column names' in the training data set.
      Label is the value we want to predict. The answer we get from our model after training.
      
      
<p align="center">
<img  height="300" src="https://github.com/pauloreis-ds/Paulo-Reis-Ciencia-de-dados/blob/master/3%20-%20An%C3%A1lise%20de%20dados%20(com%20Machine%20Learning)%20-%20Data%20Analysis%20(Machine%20Learning)/just_images/feature_label.png">
</p>

The application of ML algorithms is limited to:
      
      - Separate training (features - X) and test data (labelS - y)
            - Training_X and Training_y  
            - Test_X and Test_y  
      - Create the model
            - Choose the most suitable.
            - Create the model's object() to access its methods.
            - Pass the training data into its 'fit()' (training algorithm) method.
            - Make predictions with/about the test data.
            - Check the accuracy of the model by comparing the test data with the responses provided by the algorithm.
      

Training (X and y): act on the model (makes it learn the pattern on the data).

Test (X and y): validate the model.

The training resources are the data we provide to our model during training, along with the correct answers. The goal is for the model to map between features and labels.

The test subset is used to evaluate the trained model. **The model is not allowed to see the responses to the test suite and must make predictions using training resources only**.
We know the answers to the test set so that we can compare the test predictions with the answers.

<p align="center">
<img  height="300" src="https://github.com/pauloreis-ds/Paulo-Reis-Ciencia-de-dados/blob/master/3%20-%20An%C3%A1lise%20de%20dados%20(com%20Machine%20Learning)%20-%20Data%20Analysis%20(Machine%20Learning)/just_images/feature_label1.png">
</p>

Check this out: https://whimsical.com/CA7f3ykvXpnJ9Az32vYXva
