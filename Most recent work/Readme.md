# Collections of most recent development of Contextual Bandit and Off-policy Evaluation
**Posted by Gostab, NYU**

## *Working Path*
-We will be investigating some work done by one of the most widely cited scholors(Cornell, MIT, and Neflix & Columbia University). The link of all paper work can be found here or the child folder in this working space

### Domain Adaptation and Distribution Shift

#### **A**. *Domain Adaptation Formulation of Causal Representation Learning*

|   Author    | Paper         |      Year     |
|-------------| ------------- | ------------- |
|Uri Shalit. etl|Learning Representations for Counterfactual Inference|[2016](https://arxiv.org/pdf/1605.03661.pdf)|


#### **B**. *Follow-up articles and research on Domain Adaptation*

|   Author    | Paper         |      Year     |
|-------------| ------------- | ------------- |
|Kun Zhang, etl| Low-Dimensional Density Ratio Estimation|[2019](http://proceedings.mlr.press/v89/stojanov19a/stojanov19a.pdf) |
|  |Domain Adaptation as a Problem of Inference on Graphical Models  |[2020](https://arxiv.org/pdf/2002.03278.pdf)|
||Domain Adaptation with Invariant Representation Learning: What Transformations to Learn?|[2021](https://proceedings.neurips.cc/paper/2021/file/cfc5d9422f0c8f8ad796711102dbe32b-Paper.pdf)
|Yuta,Saito|Causal Embedding for Recommendation|[2018](https://arxiv.org/pdf/1706.07639)|
||Domain Adversarial Matrix Factorization|[2022](https://usaito.github.io/files/IJCAI2022_DAMF.pdf)|
|| Estimating individual treatment effect: generalization bounds and algorithms|[2016](https://arxiv.org/pdf/1606.03976.pdf)|

#### **C**. *Theory that forms domain-adaptation: dsitribution ratio estimate*

Note: although most papers regarding domain adaptation introduce fundamentals of covariates shift, I still recommend readers to check a few of the most renown articles that contribute a lot of work to domain adaptation.Based my understanding, **distribution ratio fitting method** is most understandable. 

*Please use the following as your reference to understand the mathematical notations and proof*

|   Author    | Paper         |      Year     |
|-------------| ------------- | ------------- |
|              | Density-ratio matching under the Bregman divergence  | [2012](https://www.ism.ac.jp/editsec/aism/pdf/10463_2011_Article_343.pdf) |
|             |Kernel Moment Matching|[2009](https://is.mpg.de/fileadmin/user_upload/files/publications/shift-book-for-LeEtAl-webversion_5376[0].pdf)|
|             |Probabiltiy Density Matching| [2008](https://link.springer.com/article/10.1007/s10463-008-0197-x#citeas),[2009](https://www.jstage.jst.go.jp/article/ipsjtcva/1/0/1_0_183/_pdf/-char/ja), [2010](https://www.jstage.jst.go.jp/article/ipsjtcva/1/0/1_0_183/_pdf/-char/ja),[2012 Book](https://yosinski.com/mlss12/media/slides/MLSS-2012-Sugiyama-Density-Ratio-Estimation-in-Machine-Learning.pdf) |
|             |Density Ratio-fitting|[2009](https://www.jmlr.org/papers/volume10/kanamori09a/kanamori09a.pdf?ref=https://githubhelp.com)|
|             |Probablistic Classification Matching| [1998](https://academic.oup.com/biomet/article-abstract/85/3/619/229087?redirectedFrom=PDF),[2004](https://projecteuclid.org/journals/bernoulli/volume-10/issue-4/Semiparametric-density-estimation-under-a-two-sample-density-ratio-model/10.3150/bj/1093265631.full)|

#### **C.Appendix**. *Some supporting documents that help you understand error bound/feature map*

Note: To make this document more reader-friendly, albeit some proof provided in one or more articles has been explicitely introduced, many math-intense technical terms, however, prelude most beginers from getting a full intake of those methods. I would say that a central interest and necessity is to justify estimators we used have statistical guarantee in convergence rate, bounded error and measures. For this very reason, I also listed some materials that I hope is useful.




### Off-line Reinforcement Learning 
[*Minmin Chen, Yuta Saito, Longqi Yang*]

Note: Off-line reinforcement learning in recommendation systems is deemed a very broad topic for which its theories and applications might be varying among a number of fields: off-line policy evaluation, counterfactual learnig, counterfactual causal effect estimating and language models. We just follow the trajectory of three representitives in bandit, off-policy evaluation and recommendation systems. 

Minmin is a current senior researcher working on contextual bandit recom-sys at Google Brain. 

[Minmin Chen(click for Google Scholar Profile)](https://mchen24.github.io/)

|   Author    | Paper         |      Year     |
|-------------| ------------- | ------------- |
||Actor Critic Methods for Off-line Policy Evaluation|[2022](https://dl.acm.org/doi/pdf/10.1145/3523227.3546758)|
||Top K Off-line Evaluaitons|[2021](https://arxiv.org/pdf/1812.02353.pdf)|


[Yuta Saito(Click for Google Page)](https://scholar.google.com/citations?user=pw4hwS8AAAAJ&hl=en) and [Thorsten Joachims](https://scholar.google.com/citations?hl=en&user=5tk1PV8AAAAJ&view_op=list_works&sortby=pubdate)

|   Author    | Paper         |      Year     |
|-------------| ------------- | ------------- |
|| Unbiased Recommendation Learning From MCNR |[2020](https://dl.acm.org/doi/pdf/10.1145/3336191.3371783)  |
||Asymmetric Tri-training for Debiasing Missing-Not-At-Random Explicit Feedback|[2020](https://arxiv.org/pdf/1910.01444.pdf)|
|| Open Bandit Database and Pipeline: Reproducible Off-line Policy Evaluation  |[2022](https://arxiv.org/abs/2008.07146)|

### Class of Inverse Propensity Score Methods

Some advanced methods are based on the most classic paper:  [The central role of the propensity score in observational studies for causal effect](https://watermark.silverchair.com/70-1-41.pdf?token=AQECAHi208BE49Ooan9kkhW_Ercy7Dm3ZL_9Cf3qfKAc485ysgAAAsQwggLABgkqhkiG9w0BBwagggKxMIICrQIBADCCAqYGCSqGSIb3DQEHATAeBglghkgBZQMEAS4wEQQMMdOqYPzH71eGJJl1AgEQgIICd_WRXQV_hVYdvvmD0RT6VfCyvv_kaoJLHfGrDiKrZ7Lrs1Uz65HKE28kGmjZqDK0ES2jLv5JWujme83nlV2ckjxBGxjCxLzuo0zTOkApaMfKG3HyYjBt1tlG850EwWebTV6Bff5aKWZfqfHIGaHZNppjYfNrTfg-HgtwOZr2fQLwY_4EeA8LwoqU9rUakYY9cIvzr8a1JMWVAWSMyY-NqyjpQ5whBKrHNZ3w0S1YxYQHdWohTDALndD_q0bnW_tVZzg8stROmItW4foyxce_YDKffqPSuqEqDC8QgKGkwyxBDZvQ7i515D6YxQktAi2putxVaZ5AbY99jItIRaOwdIqa9MT2jc3CNC1o0V7f1oI3eQoAW7l-sL-wSE6UXZFKkx5f0vtcbJrS_L2o_KYS__eLjiPjivAFHpNR5kxOstga6LcggZgw-igbTFAXPiD75BKTxnJpuJUeoTtNOkdOOWD7oojtHDqIk8-IytsDTFTV7YSkK8WIODXPAr4i_qJcsSjXtICjTwFAFpIa3z5-nTszWdq5kTsmVv8GF_iuQAdAxbvWaFGOKg0FE2x-Ia7R-QKAtptI1P_X4VKnZb-roh33ap1A2LEHcWYaUhxjh0pneFoy4Ap55y7k7hknbgwfoNJPUWgUjxlrOQBHTGkfVPg4RBMrZ2s9J0iQuEfMhe18uZTjNRzuisXxiHxMvu6vrwzYWGxRJFmuvZA5N_O00u_tBflHNu2gHJ-ImUSEpQwsIFolPjwNqpND2y7LsP1VhEMVWnUNMxs6OZKFrYFPgf98kaGKOPLHtJIKJAYuCEcaGaaTDrm8bD3R0N9FuxThVKp-lYik9Is). This paper introduced how propensity score can eliminate the overt bias by balancing the observed covariates as a balancing score and this is the finest balancing score among a class of possible balancing scores $b(x)$. The proof is straightforward and thus this document will just mention it for completeness.


1) *Batch Learning in Off-line Policy Evaluation*
2) *Self-normalized Estimator for Counterfactual Learning*(Propensity Overfitting)
3) *Double-Robust Method in Counterfactual Learning*
4) *Clipped Inverse Propensity Score*(Upper Bound $M$ method)
5) *Unbiased Off-line Reinforcement Learning MCNR*



|   Author    | Paper         |      Year     |
|-------------| ------------- | ------------- |
