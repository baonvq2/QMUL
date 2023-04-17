The project has two separate components:


1.   **Basic component** [6 marks]: Using the MLEnd London Sounds dataset, build a machine learning pipeline that takes as an input an audio segment and predicts whether the audio segment has been recorded indoors or outdoors.

The problem of the basic solution is to try to predict whether the audio file was record indoor or outdoor. So, this is a classification problem, whose target class (the one which we try to predict) is a binary variable - indoor/outdoor.
To formulate the problem of basic component in a summary view with below steps:

Problem Input: Audio data, acting as predictors (including the audio file and other related information such as areas or
Model: A machine learning (ML) model which would be used to predict the output from the given input
Problem Output: Binary class - indoor or outdoor
==> Result: avg accuracy = 0.59

2.   **Advanced component** [10 marks]: Formulate your own machine learning problem and build a machine learning solution using the MLEnd London Sounds dataset.
The problem of the basic solution is to try to predict an area where a certain audio file was record. So, this is a multi- class classification problem, whose target class (the one which we try to predict) is a variable of areas - campus/westend/british/southbank/Euston/kensington.
To formulate the problem of basic component in a summary view with below steps:

Problem Input: Audio data, acting as predictors (including the audio file and other related information such as areas or
Model: A machine learning (ML) model which would be used to predict the output from the given input
Problem Output: A predicted area where the an audio was taken
==> Result: avg. accuracy = ~43%
