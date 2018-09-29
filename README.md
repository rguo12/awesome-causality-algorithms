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

### Learning Causal Effects with Back-door Criterion
Propensity Score Matching [Python](https://github.com/akelleh/causality/tree/master/causality/estimation) </br>
Inverse Probability Reweighting [R](https://github.com/cran/ipw) </br>
Nonparametric Regression Adjustment [Python](https://github.com/akelleh/causality) </br>

Doubly Robust Estimation [R](https://github.com/gregridgeway/fastDR) </br>
Doubly Robust Estimation for High Dimensional Data [R](https://github.com/jantonelli111/DoublyRobustHD) </br>

Counterfactual Regression and CFRnet [Python](https://github.com/oddrose/cfrnet) </br>
CEVAE [Python](https://github.com/AMLab-Amsterdam/CEVAE) </br>

#### Learning Heterogeneous Causal Effects
Meta-learners for Estimating Heterogeneous Treatment Effects using Machine Learning [R](https://github.com/soerenkuenzel/hte) </br>
Causal Forest [R](https://github.com/grf-labs/grf) [Python](https://github.com/kjung/scikit-learn) </br>


#### Learning Causal Effects under Spillover Effect
LCVA [Python](https://github.com/rguo12/CIKM18-LCVA)

#### Learning Time Varying/Dependent Causal Effects
Longitudinal Targeted Maximum Likelihood Estimation [R](https://github.com/joshuaschwab/ltmle) </br>

#### Variable Selection/Importance for Learning Causal Effects
Variable importance through targeted causal inference [R](https://github.com/ck37/varimpact) </br>

### Learning Causal Effects without Back-door Criterion
#### Instrumental Variables
DeepIV [Python](https://github.com/jhartford/DeepIV) </br>
PDSLasso [STATA](https://statalasso.github.io/)

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
### Invariant Prediction
A Simple Algorithm for Invariant Prediction [Julia](https://github.com/richardkwo/InvariantCausal.jl)
