# NN-LOL-Prediction
Neural Network to predict win or lose in a League of Legends game based on previous match history

# API
Get your API KEY from [Riot Games Website](https://developer.riotgames.com). Make sure to change your summoner name and account region inside the notebook.

# CSV
In the `csv` folder there are two examples to work with. [Link](https://github.com/MatteoFasulo/NN-LOL-Prediction/blob/main/csv/example1.csv)

# Features
Some dataset features were not considered for the model. Feel free to use in case you want to carry out some analysis concerning them.

# Convergence
The proposed network achieves an accuracy of 0.89 on the validation set. As some features of the dataset have a different scale (e.g goldEarned), the dataset has been normalized through Z-score normalization. Binary crossentropy with Adam optimizer was used after finding the optimal learning rate. Finally, the model was trained with the new learning rate on a lower number of epochs to avoid overfitting.

![Accuracy and Loss](https://github.com/MatteoFasulo/NN-LOL-Prediction/blob/main/img/acc_loss.svg?raw=true "Accuracy and Loss Plot")

# Model Graph
![Model Graph](https://github.com/MatteoFasulo/NN-LOL-Prediction/blob/main/img/model.png?raw=true "Neural Network Plot")
