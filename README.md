# PacManAI
This project implements a Deep Q-Learning (DQN) agent to play the classic arcade game Ms. Pac-Man using PyTorch and OpenAI's Gymnasium environment. The agent is trained using a Convolutional Neural Network (CNN) to approximate the Q-function, which is used to determine the best actions to take in the game environment.

# Features
- Convolutional Neural Network (CNN): The agent uses a CNN with four convolutional layers followed by fully connected layers to process the game screen and predict Q-values for each possible action.
- Experience Replay: The agent stores past experiences in a replay memory and samples from it to learn, which helps to break correlation between consecutive experiences and stabilize training.
- Target Network: A separate target network is used to generate target Q-values, reducing oscillations and divergence during training.
- Epsilon-Greedy Policy: The agent follows an epsilon-greedy policy for action selection, balancing exploration and exploitation during training.
- Training Loop: The agent is trained over multiple episodes, with the goal of achieving an average score of 500+ over 100 consecutive episodes.
- Model Saving: The trained model is saved once the environment is considered solved (i.e., when the average score exceeds 500 over 100 episodes).

# Installation

Install Gymnasium and necessary packages:

- pip install gymnasium
- pip install "gymnasium[atari, accept-rom-license]"
- apt-get install -y swig
- pip install gymnasium[box2d]
