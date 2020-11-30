# RL Project: Training Flappy Bird using Double Dueling Deep Q Network [D3QN]

![Gameplay](https://github.com/s-c-soma/flappy-bird-deep-q-learning/blob/master/screenshots/gameplay.gif)


## Summary
## D3QN Network
![D3QN Network](https://cdn-images-1.medium.com/max/1200/1*FkHqwA2eSGixdS-3dvVoMA.png)

## Folder Structure and Files 
    .
    ├── assets                                                  # Contains the required audio and image files
    ├── colab                                                   # Contains the colab files
    │   ├── Flappy_DoubleDueling_DQN.ipynb                      # Colab for training model in local Jupyter Noebook
    │   └── Flappy_DoubleDueling_DQN_GoogleColab.ipynb          # Colab for training model in Google colab and code from Google Drive
    ├── cuda_check                                              
    │   └── cuda_check.py                                       # File to check local cuda setup
    ├── game                                                    # Contains the code for Flappy Bird set up with Pygame
    │   ├── flappy_utils.py                      
    │   └── flappy_wrapped.py          
    ├── model                                              
    │   └── 1_best_flappy_model.dat                             # Infinity Glappy Bird agent model trained with D3QN 
    ├── result_csv                                              
    │   └── d3qn_mean reward.csv                                # CSV file containing Mean Reward from D3QN Best Model
    ├── screenshots                                             # Contains Gif file used in readme file
    ├── runs                                                    # Tesnorboard log files
    ├── documents                                               # Contains ppt presentation and project report
    ├── play_game.py                                            # Python file to run the model from 'model' folder
    └── README.md

## Setup Environment
For environment setup please use Python version 3.x.x and setup the required packages from requirements.txt

> pip install -r requirements.txt

## Running The Game
Execute the following command to run the trained model from 'model' folder. Here '--model' indicates the location of saved D3QN model.
> python play_game.py --model model/1_best_flappy_model.dat

## Training Result
![Training Plot](https://github.com/s-c-soma/flappy-bird-deep-q-learning/blob/master/screenshots/d3qn_trainingplot.png?raw=true "D3QN Training Plot for Infinity Model")


## Acknowledements
