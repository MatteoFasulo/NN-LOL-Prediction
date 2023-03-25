# NN-LOL-Prediction
Neural Network to predict win or lose in a League of Legends game based on previous match history

# API
Get your API KEY from [Riot Games Website](https://developer.riotgames.com). Make sure to change your summoner name and account region inside the notebook.

# CSV
In the `csv` folder there is an example of match history of the last 100 games to work with. [Link](https://github.com/MatteoFasulo/NN-LOL-Prediction/blob/main/csv/example.csv)

# Convergence
The proposed network achieves an accuracy of 0.81 on the validation set with less than 200 training instances. Binary crossentropy with Adam optimizer was used after finding the optimal learning rate. Finally, the model was trained with the new learning rate on a lower number of epochs to avoid overfitting

# Model Graph
![Model Graph](https://github.com/MatteoFasulo/NN-LOL-Prediction/blob/main/code/model.png?raw=true "Neural Network Plot")
