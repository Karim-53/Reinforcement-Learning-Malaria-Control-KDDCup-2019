# Reinforcement-Learning-Malaria-Control-KDDCup-2019
KDDCup 2019: Reinforcement Learning Challenge | LOLs team's solution ranked 7th



This Repo regroup different ML solutions for the KDDCup Challenge 2019 | Policy Learning for Malaria Control.
These solutions were created by Lols team (ranked 7)

<p align="center">
  <img src="https://github.com/Karim-53/Reinforcement-Learning-Malaria-Control-KDDCup-2019/blob/master/include/kdd_comp_image.jpg">
</p>

These solutions are based on Bayesian Optimisation techniques (Upper bound confidence) (todo add link to the original repo)

<p align="center">
<figure>
  <img width="280" src="https://github.com/Karim-53/Reinforcement-Learning-Malaria-Control-KDDCup-2019/blob/master/include/y1.png">
  <figcaption>Fig.1 - Reward distribution for Year 1 (1600 points used)</figcaption>
</figure>

<figure>
  <img width="300" src="https://github.com/Karim-53/Reinforcement-Learning-Malaria-Control-KDDCup-2019/blob/master/include/y1_BO.png">
  <figcaption>Fig.2 - Reward estimation using Bayesian Optimisation (89 points used)</figcaption>
</figure>
</p>

the 3 most important solutions are:

### BO.1: BO with breaking sequence
This model uses 5 independents Bayesian Optimisation Objects. It focuses on maximizing the reward in a sequential way, starting from year 1.
 
### BO.2: 10 dimensional BO
This model uses only one Bayesian Optimisation Object. It is able to understand complex patterns between years and is able to model relations between the current reward and previously taken actions.

### BO.3: boosting network
This model combines the 2 previous algorithms thanks to the Ensemble learning techniques. It offers a more stable result: the worst case is always better than BO.1 and BO.2

<p align="center">
  <img src="https://github.com/Karim-53/Reinforcement-Learning-Malaria-Control-KDDCup-2019/blob/master/include/BO_3.png">
</p>