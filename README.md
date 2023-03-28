# NN-LOL-Prediction
Neural Network to predict win or lose in a League of Legends game based on previous match history

# API
Get your API KEY from [Riot Games Website](https://developer.riotgames.com). Make sure to change your summoner name and account region inside the notebook.

# CSV
In the `csv` folder there are two examples to work with. [Link](https://github.com/MatteoFasulo/NN-LOL-Prediction/blob/main/csv/example1.csv)

# Features
Some dataset features were not considered for the model. Feel free to use in case you want to carry out some analysis concerning them.

# Convergence
The proposed network achieves an accuracy of 0.89 on the validation set. As some features of the dataset have a different scale (e.g goldEarned), the dataset has been normalized through [Z-score normalization](https://en.wikipedia.org/wiki/Standard_score). [Binary crossentropy](https://www.tensorflow.org/api_docs/python/tf/keras/losses/BinaryCrossentropy) with [Adam optimizer](https://optimization.cbe.cornell.edu/index.php?title=Adam) was used after finding the optimal [learning rate](https://en.wikipedia.org/wiki/Learning_rate). Finally, the model was trained with the new learning rate on a lower number of epochs to avoid overfitting.

![Accuracy and Loss](https://github.com/MatteoFasulo/NN-LOL-Prediction/blob/main/img/acc_loss.svg?raw=true "Accuracy and Loss Plot")

# Model Graph
![Model Graph](https://github.com/MatteoFasulo/NN-LOL-Prediction/blob/main/img/model.png?raw=true "Neural Network Plot")

# References
1. [@SION1225 - Predict LOL Ranked game with Keras](https://www.kaggle.com/code/sion1225/predict-lol-ranked-game-with-keras-72-accuracy)
2. @GitMarco27 - [Get Teamfight Tactics (TFT) data with Python and Riot Games API](https://marcosanguineti.medium.com/get-teamfight-tactics-tdf-data-with-python-and-riot-games-api-e3243e3c54dc)
3. @RiotGames - [League of Legends API Docs](https://developer.riotgames.com/docs/lol)
