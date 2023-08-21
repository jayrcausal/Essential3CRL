# Learning Policy with 3CRL

## Section Outline

>This module is the central focus of 3CRL as it gives a big picture of the most recent off-policy/offline reinforcement leanring under different frameworks.
Albeit that conventioanl methods in Causal Inference arises in most situations where experiments are not feasibly scheduled, it still has some affinities with
offline reinforcement learning. In the paper [Causal Machine Learning|Causal Machine Learning:A Survey and Open Problems](https://arxiv.org/pdf/2206.15475.pdf)
we have highlighted, the term " offline" corresponds to many conventional Causal Inference questions: we get a data realization or sample from an
unknown distribution. Following what we have investigated in *Fundamental*, two unknown distribution or policies could be easily defined as the full-control distrbution and full-treated distribution or policy. Here I just use a oversimplified example to connect offline reinforcement learning and conventional causal inference. In this section, we will present a relatively thorough investigation onto offline reinforcement learning.
<hr>

## Overview of Offline Reinforcement Learning

Some concepts in Offline Reinforcement Learning are jointly appearing in contextual bandit with small deviation because of  replacing contexts with *trajectory distribution*. This document mainly follows the work pertaining to **Offline Reinforcement Learning** and its revevant term **trajectory Distribution**. Just in my study, what confused my a lot is the use of Partially Observed Markov Decision Process. Therefore, I plan to address this concern by putting more ink in what POMDP is and how it is related to our problem.





|   Field     | Publication   | Year          |
|-------------| ------------- | ------------- |
|Overview|**Offline Reinforcement Learning: Tutorial, Review,and Perspectives on Open Problems**|[2020](https://arxiv.org/pdf/2005.01643.pdf)|
|Q-Learning|||
|Actor-critic|||
|RL-Dynamics Programming|||