# NN-LOL-Prediction
Neural Network to predict win or lose in a League of Legends game based on previous match history

# API
Get your API KEY from [Riot Games Website](https://developer.riotgames.com). Make sure to change your summoner name and account region inside the notebook.

# Convergence
Since the match history refers only to the last 100 games, the dataset is very small and there are problems of numerical instability due to the small dataset. It would be advisable to aggregate the data of several games of different players to be able to make the model generalize in the appropriate way.
