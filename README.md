# Reinforcement-Learning-Advance-Exercise

This repository sharing my practice on Reinforcement Learning (RL) in the VIZDOOM http://vizdoom.cs.put.edu.pl by different RL methods.

### Different Environments provided in VIZDOOM:
1. Basic
2. Deadly Corridor

### Logs:

2022-04-05 Uploaded ***Reward Shaping and Curriculum Learning in Reinforcement Learning - 220409.ipynb***

***Executive Summary:***

In this notebook, I'm using ***the environment in the ViZDoom - Deadly Corridor*** to ***practice how to apply Reward Shaping and Curriculum Learning reinforcement learning***. The purpose of the Deadly Corridor scenario is to ***teach the agent to navigate towards his fundamental goal*** (the vest) and ***make sure he survives at the same time***. The ***reward formula*** in this notebook is ***(movement_reward) + (health_delta * 10) + (HITCOUNT_delta * 300) + (ammo_delta * 5)***. To ***use HITCOUNT instead of HITS_TAKEN*** are the key successful factor during the learning process. Right after ***applied 1.5 million timesteps of curriculum learning in 5 difference levels of difficulty of learning***, the ***agent received average reward: 420 in level 5 of difficulty***. Although ***the player didn't reach the goal*** (the vest), but ***it keep moving forward quickly*** and ***taking shoots during the game***. 

----------------------------------------------------------------------------------------------------------

2022-04-05 Uploaded ***VIZDoom - Basic - 220405.ipynb***

<img src='http://vizdoom.cs.put.edu.pl/user/pages/01.tutorial/basic.png' width='250px'/>

***Executive Summary:***

In this notebook, ***the goal of the Basic environment is to kill the monster as soon as possible***. First, I started with taken random actions ***The reward received in between -365 to 66 (average -121)***. After that, I used ***stable_baselines3 PPO model to train the Agent*** in order to complete this goal. As a result, The ***Mean Reward reach highest reward at 150k timesteps around 80*** (time spend 1hr 18min), ***the agent perform significantly better and it killed the monster very quickly***.

----------------------------------------------------------------------------------------------------------
