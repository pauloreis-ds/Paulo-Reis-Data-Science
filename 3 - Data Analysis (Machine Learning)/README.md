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
    so that It knows what to do with each data that we enter. So that It knows how to classify them.

    > Briefly explained, a feature would be the input data that you provided to the system and the 
      label would be the output (the answer/prediction) that is expected.
      
    Example: classifying/predicting geometric figures.

                         (input)                                                    (output)
    features = [number_of_sides, number_of_diagonals...]  -->  Model(features)  -->  Hexagon 
    

    > Features are patterns, colors, shapes... that is, 'column names' in the training data set.
      Label is the value we want to predict. The answer we get from our model after training.
      
      
<p align="center">
<img  height="300" src="https://github.com/pauloreis-ds/Paulo-Reis-Ciencia-de-dados/blob/master/3%20-%20An%C3%A1lise%20de%20dados%20(com%20Machine%20Learning)%20-%20Data%20Analysis%20(Machine%20Learning)/just_images/feature_label.png">
</p>

The application of ML algorithms is "limited" to:
      
      - Separate training (features = X) and test data (labels - y)
            - Training_X and Training_y --> The model will learn the (mathematical) relationship between them.  
            - Test_X and Test_y --> After that, We can see if it's done right.  
      - Create the model
            - Choose the most suitable.
            - Create the model's object() to access its methods.
            - Pass the training data into its 'fit()' (training algorithm) method.
            - Make predictions with/about the test_X data.
            - Check the accuracy of the model by comparing the test_y data with the responses provided by the algorithm.
      

Training (X and y) acts on the model (makes it learn the pattern on the data).

Test (X and y) validates the model.

The training resources/features (training_X) are the data we provide to our model during training, along with the correct answers/labels (training_y). The goal is for the model to map between features and labels.

The test subset is used to evaluate the trained model. **The model is not allowed to see the responses to the test suite and must make predictions using only the learnings from the training resources learning**.
We know the answers to the test set so that we can compare the test predictions with the answers.

<p align="center">
<img  height="300" src="https://github.com/pauloreis-ds/Paulo-Reis-Ciencia-de-dados/blob/master/3%20-%20An%C3%A1lise%20de%20dados%20(com%20Machine%20Learning)%20-%20Data%20Analysis%20(Machine%20Learning)/just_images/feature_label1.png">
</p>

Check this out: https://whimsical.com/CA7f3ykvXpnJ9Az32vYXva
