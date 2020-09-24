# Reinforcement-Learning-Malaria-Control-KDDCup-2019
**KDDCup 2019: Reinforcement Learning Challenge | LOLs team's solution ranked 7th**

We were selected to represent Passau University during this RL Competition. A [paper](https://arxiv.org/abs/1910.08926 "Arxiv pdf") resuming our work was afterward
published.

This Repo regroup different ML solutions for the KDDCup Challenge 2019 | Policy Learning for Malaria Control.
These solutions were created by Lols team (ranked 7)

<p align="center">
  <img src="https://github.com/Karim-53/Reinforcement-Learning-Malaria-Control-KDDCup-2019/blob/master/include/kdd_comp_image.jpg">
</p>

These solutions are based on Bayesian Optimisation techniques (Upper bound confidence) (todo add link to the original repo)

 <div>
           <div style="width:80%;Text-align:center;float:left;">
         
<figure style="width:25%;float:left;margin:0px;text-align:center;padding:0px;">
  <img width="280" src="https://github.com/Karim-53/Reinforcement-Learning-Malaria-Control-KDDCup-2019/blob/master/include/y1.png">
  <figcaption>Fig.1 - Reward distribution for Year 1 (1600 points used)</figcaption>
</figure>
  
</div>
           
<div style="Text-align:right;Width:20%;float:right">
           
<figure style="width:25%;float:left;margin:0px;text-align:center;padding:0px;">
  <img width="300" src="https://github.com/Karim-53/Reinforcement-Learning-Malaria-Control-KDDCup-2019/blob/master/include/y1_BO.png">
  <figcaption>Fig.2 - Reward estimation using Bayesian Optimisation (89 points used)</figcaption>
</figure>

</div>


</div>
           



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


## Litereture
bibtex to our paper:
```
@article{nguyen2019policy,
  title={Policy learning for malaria control},
  author={Nguyen, Van Bach and Karim, Belaid Mohamed and Vu, Bao Long and Schl{\"o}tterer, J{\"o}rg and Granitzer, Michael},
  journal={arXiv preprint arXiv:1910.08926},
  year={2019}
}
```
