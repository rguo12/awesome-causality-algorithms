# awesome-causality-algorithms
An index of algorithms for learning causality with data.

Please cite our survey if this index is helpful.

@article{guo2018survey,</br>
  title={A Survey of Learning Causality with Data: Problems and Methods},</br>
  author={Guo, Ruocheng and Cheng, Lu and Li, Jundong and Hahn, P. Richard and Liu, Huan}, </br>
  journal={arXiv preprint arXiv:1809.09337}, </br>
  year={2018}</br>
}

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
|---|---|---|
|Counterfactual Regression and CFRnet|Johansson, Fredrik, Uri Shalit, and David Sontag. "Learning representations for counterfactual inference." In International Conference on Machine Learning, pp. 3020-3029. 2016.|[Python](https://github.com/oddrose/cfrnet)|
|Causal Effect VAE|Louizos, Christos, Uri Shalit, Joris M. Mooij, David Sontag, Richard Zemel, and Max Welling. "Causal effect inference with deep latent-variable models." In Advances in Neural Information Processing Systems, pp. 6446-6456. 2017.|[Python](https://github.com/AMLab-Amsterdam/CEVAE)|
|SITE|Yao, Liuyi, Sheng Li, Yaliang Li, Mengdi Huai, Jing Gao, and Aidong Zhang. "Representation Learning for Treatment Effect Estimation from Observational Data." In Advances in Neural Information Processing Systems, pp. 2638-2648. 2018.|[Python](https://github.com/Osier-Yi/SITE)|
|Meta-learners for Estimating Heterogeneous Treatment Effects using Machine Learning|Künzel, Sören R., Jasjeet S. Sekhon, Peter J. Bickel, and Bin Yu. "Meta-learners for Estimating Heterogeneous Treatment Effects using Machine Learning." arXiv preprint arXiv:1706.03461 (2017).|[R](https://github.com/soerenkuenzel/hte)|
|Causal Forest|Wager, Stefan, and Susan Athey. "Estimation and inference of heterogeneous treatment effects using random forests." Journal of the American Statistical Association just-accepted (2017).|[R](https://github.com/grf-labs/grf) [Python](https://github.com/kjung/scikit-learn)|
|NSGP (Non-stationary Gaussian Process Prior)| Alaa, Ahmed, and Mihaela Schaar. "Limits of estimating heterogeneous treatment effects: Guidelines for practical algorithm design." In International Conference on Machine Learning, pp. 129-138. 2018. |NA|
|Deep Counterfactual Networks (Propensity Dropout)| Alaa, Ahmed M., Michael Weisz, and Mihaela van der Schaar. "Deep counterfactual networks with propensity-dropout." arXiv preprint arXiv:1706.05966 (2017).|NA|

#### Learning Causal Effects under Spillover Effect
LCVA [Python](https://github.com/rguo12/CIKM18-LCVA)

#### Learning Time Varying/Dependent Causal Effects
Longitudinal Targeted Maximum Likelihood Estimation [R](https://github.com/joshuaschwab/ltmle) </br>

#### Variable Selection/Importance for Learning Causal Effects
Variable importance through targeted causal inference [R](https://github.com/ck37/varimpact) </br>

### Learning Causal Effects without the Unconfoundedness Assumption
|Instrumental Variables|
|DeepIV|Hartford, Jason, Greg Lewis, Kevin Leyton-Brown, and Matt Taddy. "Deep iv: A flexible approach for counterfactual prediction." In International Conference on Machine Learning, pp. 1414-1423. 2017.|[Python](https://github.com/jhartford/DeepIV)|
|PDSLasso|   |[STATA](https://statalasso.github.io/)|

## Learning Causal Relationships
### Learning Causal Relationships with i.i.d. Data
[TETRAD toolbox](http://www.phil.cmu.edu/tetrad/about.html) [R](https://github.com/bd2kccd/r-causal)</br>
CausalDiscoveryToolbox [Python](https://github.com/Diviyan-Kalainathan/CausalDiscoveryToolbox) </br>
IC algorithm [Python](https://github.com/akelleh/causality) </br>
PC algorithm [Python](https://github.com/keiichishima/pcalg) [R](https://github.com/cran/pcalg) [Julia](https://github.com/mschauer/CausalInference.jl) </br>
FCI algorithm [R](https://github.com/cran/pcalg) </br>

#### Distinguishing Cause from Effect (Bivariate)
BMLiNGAM [Python](https://github.com/taku-y/bmlingam)

#### Conditional Independence Tests (for Constraint-based Algorithms)
RCIT [R](https://github.com/ericstrobl/RCIT)

#### Causal Discovery Meets Probabilistic Logic Programming
Causal PSL [Java](bitbucket.org/linqs/causpsl)

### Learning Causal Relationships with non-i.i.d. Data


## Connections to Machine Learning
### Recommendation as Causal Inference
|---|---|---|
|IPS Estimator|Schnabel, Tobias, Adith Swaminathan, Ashudeep Singh, Navin Chandak, and Thorsten Joachims. "Recommendations as treatments: Debiasing learning and evaluation." arXiv preprint arXiv:1602.05352 (2016).|[Python](http://www.cs.cornell.edu/~schnabts/mnar/index.html)|
### Invariant Prediction
A Simple Algorithm for Invariant Prediction [Julia](https://github.com/richardkwo/InvariantCausal.jl)
