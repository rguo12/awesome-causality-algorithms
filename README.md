# awesome-causality-algorithms
An index of algorithms for learning causality with data.

Please cite our survey if this index is helpful.
```
@article{guo2018survey,
  title={A Survey of Learning Causality with Data: Problems and Methods},
  author={Guo, Ruocheng and Cheng, Lu and Li, Jundong and Hahn, P. Richard and Liu, Huan}, 
  journal={arXiv preprint arXiv:1809.09337}, 
  year={2018}
}
```

*Updates are coming soon!*

## Learning Causal Effects

### Learning Causal Effects with Unconfoundedness Assumption

|Name|Paper|Code|
|---|---|---|
|Propensity Score Matching|   |[Python](https://github.com/akelleh/causality/tree/master/causality/estimation)|
|Inverse Probability Reweighting|   |[R](https://github.com/cran/ipw)|
|Nonparametric Regression Adjustment|   |[Python](https://github.com/akelleh/causality)|
|Doubly Robust Estimation|   |[R](https://github.com/gregridgeway/fastDR)|
|Doubly Robust Estimation for High Dimensional Data|Antonelli, Joseph, Matthew Cefalu, Nathan Palmer, and Denis Agniel. "Doubly robust matching estimators for high dimensional confounding adjustment." Biometrics (2016).|[R](https://github.com/jantonelli111/DoublyRobustHD)|
|TMLE|Gruber, Susan, and Mark J. van der Laan. "tmle: An R package for targeted maximum likelihood estimation." (2011).|[R](https://cran.r-project.org/web/packages/tmle/index.html)|
|---|---|---|
|BNN, BLR|Johansson, Fredrik, Uri Shalit, and David Sontag. "Learning representations for counterfactual inference." In International Conference on Machine Learning, pp. 3020-3029. 2016.|[Python](https://github.com/oddrose/cfrnet)|
|Tarnet, Counterfactual Regression|Shalit, Uri, Fredrik D. Johansson, and David Sontag. "Estimating individual treatment effect: generalization bounds and algorithms." arXiv preprint arXiv:1606.03976 (2016).|[Python](https://github.com/oddrose/cfrnet)|
|Causal Effect VAE|Louizos, Christos, Uri Shalit, Joris M. Mooij, David Sontag, Richard Zemel, and Max Welling. "Causal effect inference with deep latent-variable models." In Advances in Neural Information Processing Systems, pp. 6446-6456. 2017.|[Python](https://github.com/AMLab-Amsterdam/CEVAE)|
|SITE|Yao, Liuyi, Sheng Li, Yaliang Li, Mengdi Huai, Jing Gao, and Aidong Zhang. "Representation Learning for Treatment Effect Estimation from Observational Data." In Advances in Neural Information Processing Systems, pp. 2638-2648. 2018.|[Python](https://github.com/Osier-Yi/SITE)|
|Meta-learners for Estimating Heterogeneous Treatment Effects using Machine Learning|Künzel, Sören R., Jasjeet S. Sekhon, Peter J. Bickel, and Bin Yu. "Meta-learners for Estimating Heterogeneous Treatment Effects using Machine Learning." arXiv preprint arXiv:1706.03461 (2017).|[R](https://github.com/soerenkuenzel/hte)|
|Causal Forest|Wager, Stefan, and Susan Athey. "Estimation and inference of heterogeneous treatment effects using random forests." Journal of the American Statistical Association just-accepted (2017).|[R](https://github.com/grf-labs/grf) [Python](https://github.com/kjung/scikit-learn)|
|Bayesian Additive Regression Trees (BART)|Hill, Jennifer L. "Bayesian nonparametric modeling for causal inference." Journal of Computational and Graphical Statistics 20, no. 1 (2011): 217-240.||
|NSGP (Non-stationary Gaussian Process Prior)| Alaa, Ahmed, and Mihaela Schaar. "Limits of estimating heterogeneous treatment effects: Guidelines for practical algorithm design." In International Conference on Machine Learning, pp. 129-138. 2018. |NA|
|Deep Counterfactual Networks (Propensity Dropout)| Alaa, Ahmed M., Michael Weisz, and Mihaela van der Schaar. "Deep counterfactual networks with propensity-dropout." arXiv preprint arXiv:1706.05966 (2017).|NA|
|CMGP (Causal Multi-task Gaussian Processes)|Alaa, Ahmed M., and Mihaela van der Schaar. "Bayesian inference of individualized treatment effects using multi-task gaussian processes." In Advances in Neural Information Processing Systems, pp. 3424-3432. 2017.|NA|
|GANITE|Yoon, Jinsung, James Jordon, and Mihaela van der Schaar. "GANITE: Estimation of Individualized Treatment Effects using Generative Adversarial Nets." (2018).|NA|
|Differentiated Confounder Balancing (ATT/ATE only)|Kuang, Kun, Peng Cui, Bo Li, Meng Jiang, and Shiqiang Yang. "Estimating Treatment Effect in the Wild via Differentiated Confounder Balancing." In Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, pp. 265-274. ACM, 2017.|NA|
||Li, Sheng, and Yun Fu. "Matching on balanced nonlinear representations for treatment effects estimation." In Advances in Neural Information Processing Systems, pp. 929-939. 2017.|NA|

#### Learning Causal Effects under Spillover Effect
|Name|Paper|Code|
|---|---|---|
|Linked Causal Variational Autoencoder (LCVA)|Rakesh, Vineeth, Ruocheng Guo, Raha Moraffah, Nitin Agarwal, and Huan Liu. "Linked Causal Variational Autoencoder for Inferring Paired Spillover Effects." In Proceedings of the 27th ACM International Conference on Information and Knowledge Management, pp. 1679-1682. ACM, 2018.|[Python](https://github.com/rguo12/CIKM18-LCVA)|

#### Learning Time Varying/Dependent Causal Effects
|Name|Paper|Code|
|---|---|---|
|Longitudinal Targeted Maximum Likelihood Estimation|Petersen, Maya, Joshua Schwab, Susan Gruber, Nello Blaser, Michael Schomaker, and Mark van der Laan. "Targeted maximum likelihood estimation for dynamic and static longitudinal marginal structural working models." Journal of causal inference 2, no. 2 (2014): 147-185.|[R](https://github.com/joshuaschwab/ltmle)|
|Recurrent Marginal Structural Networks| Lim, Bryan. "Forecasting Treatment Responses Over Time Using Recurrent Marginal Structural Networks." In Advances in Neural Information Processing Systems, pp. 7494-7504. 2018.  |[Python](https://github.com/sjblim/rmsn_nips_2018)|

#### Variable Selection/Importance for Learning Causal Effects
Variable importance through targeted causal inference [R](https://github.com/ck37/varimpact) </br>

### Learning Causal Effects without the Unconfoundedness Assumption
#### Instrumental Variables
|Name|Paper|Code|
|---|---|---|
|DeepIV|Hartford, Jason, Greg Lewis, Kevin Leyton-Brown, and Matt Taddy. "Deep iv: A flexible approach for counterfactual prediction." In International Conference on Machine Learning, pp. 1414-1423. 2017.|[Python](https://github.com/jhartford/DeepIV)|
|PDSLasso|   |[STATA](https://statalasso.github.io/)|

## Connections to Machine Learning
### Recommendation as Causal Inference
|Name|Paper|Code|
|---|---|---|
|Causal Embedding for Recommendation|Bonner, Stephen, and Flavian Vasile. "Causal embeddings for recommendation." In Proceedings of the 12th ACM Conference on Recommender Systems, pp. 104-112. ACM, 2018.|[Python](https://github.com/criteo-research/CausE)|
|IPS Estimator|Schnabel, Tobias, Adith Swaminathan, Ashudeep Singh, Navin Chandak, and Thorsten Joachims. "Recommendations as treatments: Debiasing learning and evaluation." arXiv preprint arXiv:1602.05352 (2016).|[Python](http://www.cs.cornell.edu/~schnabts/mnar/index.html)|
|Deconfounded Recsys|Wang, Yixin, Dawen Liang, Laurent Charlin, and David M. Blei. "The Deconfounded Recommender: A Causal Inference Approach to Recommendation." arXiv preprint arXiv:1808.06581 (2018).|NA|

### Feature Selection
|Name|Paper|Code|
|---|---|---|
|Causal FS for text classification|Michael J. Paul. Feature selection as causal inference: experiments with text classification. Conference on Computational Natural Language Learning (CoNLL), Vancouver, Canada. August 2017.|NA|

### Reinforcement Learning
|Name|Paper|Code|
|---|---|---|
|Casual Bandit|Lee, Sanghack, and Elias Bareinboim. Structural Causal Bandits with Non-manipulable Variables. Technical Report R-40, Purdue AI Lab, Department of Computer Science, Purdue University, 2019.|NA|
|Counterfactual-Guided Policy Search (CF-GPS)|Buesing, Lars, Theophane Weber, Yori Zwols, Sebastien Racaniere, Arthur Guez, Jean-Baptiste Lespiau, and Nicolas Heess. "Woulda, Coulda, Shoulda: Counterfactually-Guided Policy Search." arXiv preprint arXiv:1811.06272 (2018).|NA|

### Offline Policy Evaluation
|Name|Paper|Code|
|---|---|---|
|Counterfactual Risk Minimization (POEM)|Swaminathan, Adith, and Thorsten Joachims. "Counterfactual risk minimization: Learning from logged bandit feedback." In International Conference on Machine Learning, pp. 814-823. 2015.|[Python](http://www.cs.cornell.edu/~adith/POEM/index.html)|
|Self Normalized Estimator|Swaminathan, Adith, and Thorsten Joachims. "The self-normalized estimator for counterfactual learning." In Advances in Neural Information Processing Systems, pp. 3231-3239. 2015.|[Python](http://www.cs.cornell.edu/~adith/POEM/index.html)|

### Invariant Prediction
|Name|Paper|Code|
|---|---|---|
|Deep Global Balancing Regression|Kuang, Kun, Peng Cui, Susan Athey, Ruoxuan Xiong, and Bo Li. "Stable Prediction across Unknown Environments." In Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, pp. 1617-1626. ACM, 2018.|NA|
|A Simple Algorithm for Invariant Prediction| |[Julia](https://github.com/richardkwo/InvariantCausal.jl)|



## Learning Causal Relationships
### Learning Causal Relationships with i.i.d. Data
|Name|Paper|Code|
|---|---|---|
|[TETRAD toolbox](http://www.phil.cmu.edu/tetrad/about.html)|   |[R](https://github.com/bd2kccd/r-causal)|
|CausalDiscoveryToolbox| |[Python](https://github.com/Diviyan-Kalainathan/CausalDiscoveryToolbox)|
|IC algorithm| |[Python](https://github.com/akelleh/causality)|
|PC algorithm|P. Spirtes, C. Glymour, and R. Scheines. Causation, Prediction, and Search. The MIT Press, 2nd edition, 2000.|[Python](https://github.com/keiichishima/pcalg) [R](https://github.com/cran/pcalg) [Julia](https://github.com/mschauer/CausalInference.jl)|
|FCI algorithm| |[R](https://github.com/cran/pcalg)|

#### Distinguishing Cause from Effect (Bivariate)
|Name|Paper|Code|
|---|---|---|
|BMLiNGAM|S. Shimizu and K. Bollen. Bayesian estimation of causal direction in acyclic structural equation models with individual-specific confounder variables and non-Gaussian distributions. Journal of Machine Learning Research, 15: 2629-2652, 2014.|[Python](https://github.com/taku-y/bmlingam)|

#### Conditional Independence Tests (for Constraint-based Algorithms)
RCIT [R](https://github.com/ericstrobl/RCIT)

#### Causal Discovery Meets Probabilistic Logic Programming
|Name|Paper|Code|
|---|---|---|
|Causal PSL|Sridhar, Dhanya, Jay Pujara, and Lise Getoor. "Scalable Probabilistic Causal Structure Discovery." In IJCAI, pp. 5112-5118. 2018.|[Java](https://bitbucket.org/linqs/causpsl)|

### Learning Causal Relationships with non-i.i.d. Data

