# AI agent for OpenAI Gym BlackJack environment
Reinforcement Learning project, solving BlackJack env with Monte Carlo Control.<br>
This is part of an Udacity nanodegree in Deep Reinforcement Learning.<br>
environment: OpenAI Gym BlackJack-v0<br>
<br>
## Description
BlackJack, also called 21, is a card game in which the objective is to get as close to 21 as possible, but without overtaking it. This mini-project is about creating an artificial intelligence player for the game.<br>
Differently from creating step by step instructions to play the game, i.e. hard-coded, this program uses Machine Learning. It experiments the game by itself, and increases its performance over time, in other words, it learns to play.<br>
<br>
The machine learning technique used here is called Reinforcement Learning. This name is derived from behaviour psychology. It is composed by an environment and an agent. The objective of the agent is to obtain reward, as much as possible. The learning takes place through the interaction of the agent with the environment, in a process of trial and error. The environment presents the agent states, then the agent takes an action based on the observation of that state, then the environment rewards the agent based in the action and generates a new state, and the process repeats.<br>
Below you can see an example of environment-agent interaction:<br>
<br>
import gym<br>
env = gym.make('Blackjack-v0')<br>
state = env.reset()<br>
print(state)<br>
[out](12, 3, False)<br>
<br>
The "(12, 3, False)" output means that the player has a sum of 12, the dealer has 3. "False" means the player do not have an ace.<br>
<br>
To-Do: currently the rewards are undiscounted, create and implement a discount function.
