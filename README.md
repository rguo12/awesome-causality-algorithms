# awesome-causality-algorithms [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

An index of algorithms for learning causality with data.

Please cite [our survey paper](https://arxiv.org/pdf/1809.09337) if this index is helpful.
```
@article{guo2018survey,
  title={A Survey of Learning Causality with Data: Problems and Methods},
  author={Guo, Ruocheng and Cheng, Lu and Li, Jundong and Hahn, P. Richard and Liu, Huan}, 
  journal={arXiv preprint arXiv:1809.09337}, 
  year={2018}
}
```
*Updates on Counterfactual Fairness/Explanantions 01/30/2020, PRs are welcome!*

# Table of Contents

- [Toolboxes](#toolboxes)
- [Learning Causal Effects](#learning-causal-effects)
- [Connections to Machine Learning](#connections-to-machine-learning)

## Toolboxes
|Name|Paper|Code|
|---|---|---|
|DoWhy|[Amit Sharma and Emre Kiciman. "Tutorial on Causal Inference and Counterfactual Reasoning." In ACM SIGKDD 2018](http://causalinference.gitlab.io/kdd-tutorial/)|[Python](https://github.com/microsoft/dowhy)|
|[TETRAD toolbox](http://www.phil.cmu.edu/tetrad/about.html)|[Ramsey, Joseph D., Kun Zhang, Madelyn Glymour, Ruben Sanchez Romero, Biwei Huang, Imme Ebert-Uphoff, Savini Samarasinghe, Elizabeth A. Barnes, and Clark Glymour. "TETRAD-AToolbox FOR CAUSAL DISCOVERY."](https://www.atmos.colostate.edu/~iebert/PAPERS/CI2018_paper_35.pdf)|[R](https://github.com/bd2kccd/r-causal)|
|CausalDiscoveryToolbox|[Kalainathan, Diviyan, and Olivier Goudet. "Causal Discovery Toolbox: Uncover causal relationships in Python." arXiv preprint arXiv:1903.02278 (2019).](https://arxiv.org/pdf/1903.02278)|[Python](https://github.com/Diviyan-Kalainathan/CausalDiscoveryToolbox)|
|Uber CausalML|NA|[Python](https://github.com/uber/causalml)|
|JustCause|For evaluation of heterogeneous treatment effect estimators on common reference as well as synthetic data. [Underlying thesis](https://justcause.readthedocs.io/en/latest/_downloads/e054f7a0fc9cf9e680173600cb4b4350/thesis-mfranz.pdf)|[Python](https://github.com/inovex/justcause)|

## Learning Causal Effects

### With i.i.d Data

#### For Individual-level Treatment Effects (ITEs)

|Name|Paper|Code|
|---|---|---|
|Propensity Score Matching|[Rosenbaum, Paul R., and Donald B. Rubin. "The central role of the propensity score in observational studies for causal effects." Biometrika 70, no. 1 (1983): 41-55.](https://academic.oup.com/biomet/article-pdf/70/1/41/662954/70-1-41.pdf)|[Python](https://github.com/akelleh/causality/tree/master/causality/estimation)|
|Nonparametric Regression Adjustment|   |[Python](https://github.com/akelleh/causality)|
|BNN, BLR|[Johansson, Fredrik, Uri Shalit, and David Sontag. "Learning representations for counterfactual inference." In International Conference on Machine Learning, pp. 3020-3029. 2016.](http://www.jmlr.org/proceedings/papers/v48/johansson16.pdf)|[Python](https://github.com/oddrose/cfrnet)|
|TARNet, Counterfactual Regression|[Shalit, Uri, Fredrik D. Johansson, and David Sontag. "Estimating individual treatment effect: generalization bounds and algorithms." arXiv preprint arXiv:1606.03976 (2016).](https://arxiv.org/pdf/1606.03976)|[Python](https://github.com/oddrose/cfrnet)|
|Causal Effect VAE|[Louizos, Christos, Uri Shalit, Joris M. Mooij, David Sontag, Richard Zemel, and Max Welling. "Causal effect inference with deep latent-variable models." In Advances in Neural Information Processing Systems, pp. 6446-6456. 2017.](http://papers.nips.cc/paper/7223-causal-effect-inference-with-deep-latent-variable-models.pdf)|[Python](https://github.com/AMLab-Amsterdam/CEVAE)|
|SITE|[Yao, Liuyi, Sheng Li, Yaliang Li, Mengdi Huai, Jing Gao, and Aidong Zhang. "Representation Learning for Treatment Effect Estimation from Observational Data." In Advances in Neural Information Processing Systems, pp. 2638-2648. 2018.](https://papers.nips.cc/paper/7529-representation-learning-for-treatment-effect-estimation-from-observational-data.pdf)|[Python](https://github.com/Osier-Yi/SITE)|
|X-learner|[Künzel, Sören R., Jasjeet S. Sekhon, Peter J. Bickel, and Bin Yu. "Metalearners for estimating heterogeneous treatment effects using machine learning." Proceedings of the National Academy of Sciences 116, no. 10 (2019): 4156-4165.](https://www.pnas.org/content/pnas/early/2019/02/14/1804597116.full.pdf)|[R](https://github.com/soerenkuenzel/hte)[R](https://github.com/xnie/rlearner/blob/master/R/xlearner.R)|
|Causal Forest|[Wager, Stefan, and Susan Athey. "Estimation and inference of heterogeneous treatment effects using random forests." Journal of the American Statistical Association just-accepted (2017).](https://www.tandfonline.com/doi/pdf/10.1080/01621459.2017.1319839)|[R](https://github.com/grf-labs/grf) [Python](https://github.com/kjung/scikit-learn)|
|Causal MARS, Causal Boosting, Pollinated Transformed Outcome Forests|[S. Powers et al., “Some methods for heterogeneous treatment effect estimation in high-dimensions,” 2017.](https://arxiv.org/pdf/1707.00102.pdf)|[R](https://github.com/grf-labs/grf) [R](https://github.com/saberpowers/causalLearning)|
|Bayesian Additive Regression Trees (BART)|[Hill, Jennifer L. "Bayesian nonparametric modeling for causal inference." Journal of Computational and Graphical Statistics 20, no. 1 (2011): 217-240.](https://www.tandfonline.com/doi/pdf/10.1198/jcgs.2010.08162)|[Python](https://github.com/JakeColtman/bartpy)|
|GANITE|[Yoon, Jinsung, James Jordon, and Mihaela van der Schaar. "GANITE: Estimation of Individualized Treatment Effects using Generative Adversarial Nets." (2018).](https://openreview.net/forum?id=ByKWUeWA-)|[Python](https://github.com/jsyoon0823/GANITE)|
|Perfect Match|[Schwab, Patrick, Lorenz Linhardt, and Walter Karlen. "Perfect match: A simple method for learning representations for counterfactual inference with neural networks." arXiv preprint arXiv:1810.00656 (2018)](https://arxiv.org/pdf/1810.00656)|[Python](https://github.com/d909b/perfect_match)|
|Dragonnet|[Adapting Neural Networks for the Estimation of Treatment Effects](https://arxiv.org/abs/1906.02120)|[Python](https://github.com/claudiashi57/dragonnet)|
|Active Learning for Decision-Making from Imbalanced Observational Data|[Active Learning for Decision-Making from Imbalanced Observational Data](https://arxiv.org/abs/1904.05268)|NA|
|ABCEI|[Adversarial Balancing-based Representation Learning for Causal Effect Inference with Observational Data](https://arxiv.org/pdf/1904.13335.pdf)|NA|
|NSGP (Non-stationary Gaussian Process Prior)|[Alaa, Ahmed, and Mihaela Schaar. "Limits of estimating heterogeneous treatment effects: Guidelines for practical algorithm design." In International Conference on Machine Learning, pp. 129-138. 2018.](http://proceedings.mlr.press/v80/alaa18a/alaa18a.pdf)|NA|
|CMGP (Causal Multi-task Gaussian Processes)|[Alaa, Ahmed M., and Mihaela van der Schaar. "Bayesian inference of individualized treatment effects using multi-task gaussian processes." In Advances in Neural Information Processing Systems, pp. 3424-3432. 2017.](https://papers.nips.cc/paper/6934-bayesian-inference-of-individualized-treatment-effects-using-multi-task-gaussian-processes.pdf)|NA|
|BNR-NNM(balanced and nonlinear representations-nearest neighbor matching)|[Li, Sheng, and Yun Fu. "Matching on balanced nonlinear representations for treatment effects estimation." In Advances in Neural Information Processing Systems, pp. 929-939. 2017.](http://papers.nips.cc/paper/6694-matching-on-balanced-nonlinear-representations-for-treatment-effects-estimation.pdf)|NA|
|Deep Counterfactual Networks (Propensity Dropout)|[Alaa, Ahmed M., Michael Weisz, and Mihaela van der Schaar. "Deep counterfactual networks with propensity-dropout." arXiv preprint arXiv:1706.05966 (2017)](https://arxiv.org/pdf/1706.05966)|NA|
||[Kallus, Nathan, Xiaojie Mao, and Angela Zhou. "Interval Estimation of Individual-Level Causal Effects Under Unobserved Confounding." In The 22nd International Conference on Artificial Intelligence and Statistics, pp. 2281-2290. 2019.](https://arxiv.org/abs/1810.02894)|NA|
|Multiple Responses in Uplift Models|[Weiss, Sam. Estimating and Visualizing Business Tradeoffs in Uplift Models](https://medium.com/building-ibotta/estimating-and-visualizing-business-tradeoffs-in-uplift-models-80ff845a5698) |[Python](https://github.com/Ibotta/mr_uplift)|

#### For Average-level Treatment Effects: ATE, ATT or ATC
|Name|Paper|Code|
|---|---|---|
|Inverse Probability Reweighting|[Rosenbaum, Paul R., and Donald B. Rubin. "The central role of the propensity score in observational studies for causal effects." Biometrika 70, no. 1 (1983): 41-55.](https://academic.oup.com/biomet/article-pdf/70/1/41/662954/70-1-41.pdf)|[R](https://github.com/cran/ipw)|
|Doubly Robust Estimation|[Bang, Heejung, and James M. Robins. "Doubly robust estimation in missing data and causal inference models." Biometrics 61, no. 4 (2005): 962-973.](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1541-0420.2005.00377.x)   |[R](https://github.com/gregridgeway/fastDR)|
|Doubly Robust Estimation for High Dimensional Data|[Antonelli, Joseph, Matthew Cefalu, Nathan Palmer, and Denis Agniel. "Doubly robust matching estimators for high dimensional confounding adjustment." Biometrics (2016).](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6347556/)|[R](https://github.com/jantonelli111/DoublyRobustHD)|
|TMLE|[Gruber, Susan, and Mark J. van der Laan. "tmle: An R package for targeted maximum likelihood estimation." (2011).](https://www.jstatsoft.org/article/view/v051i13)|[R](https://cran.r-project.org/web/packages/tmle/index.html)|
|Entropy Balancing|[Hainmueller, Jens. "Entropy balancing for causal effects: A multivariate reweighting method to produce balanced samples in observational studies." Political Analysis 20, no. 1 (2012): 25-46.](https://www.jstor.org/stable/pdf/41403737.pdf)|[R](https://github.com/cran/ebal)|
|CBPS(Covariate Balancing Propensity Score)|[Imai, Kosuke, and Marc Ratkovic. "Covariate balancing propensity score." Journal of the Royal Statistical Society: Series B (Statistical Methodology) 76, no. 1 (2014): 243-263.](https://rss.onlinelibrary.wiley.com/doi/full/10.1111/rssb.12027)|[R](https://github.com/kosukeimai/CBPS)|
|Approximate Residual Balancing|[Athey, Susan, Guido W. Imbens, and Stefan Wager. "Approximate residual balancing: debiased inference of average treatment effects in high dimensions." Journal of the Royal Statistical Society: Series B (Statistical Methodology) 80, no. 4 (2018): 597-623.](https://rss.onlinelibrary.wiley.com/doi/pdf/10.1111/rssb.12268)|[R](https://github.com/swager/balanceHD)|
|Differentiated Confounder Balancing|[Kuang, Kun, Peng Cui, Bo Li, Meng Jiang, and Shiqiang Yang. "Estimating Treatment Effect in the Wild via Differentiated Confounder Balancing." In Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, pp. 265-274. ACM, 2017.](http://media.cs.tsinghua.edu.cn/~multimedia/cuipeng/papers/CausalDCA.pdf)|NA|
|Adversarial Balancing|[Ozery-Flato, Michal, Pierre Thodoroff, and Tal El-Hay. "Adversarial Balancing for Causal Inference." arXiv preprint arXiv:1810.07406 (2018).](https://arxiv.org/pdf/1810.07406)|NA|
|DeepMatch|[Kallus, Nathan. "Deepmatch: Balancing deep covariate representations for causal inference using adversarial training." arXiv preprint arXiv:1802.05664 (2018).](https://arxiv.org/pdf/1802.05664)|NA|

#### Treatment Responder Classification
|Name|Paper|Code|
|---|---|---|
|RespSVM|[Kallus, Nathan. "Classifying Treatment Responders Under Causal Effect Monotonicity." arXiv preprint arXiv:1902.05482 (2019)](https://arxiv.org/pdf/1902.05482.pdf)|NA|

#### Learning Causal Effects as Response Curves
|Name|Paper|Code|
|---|---|---|
|Dose response networks (DRNets)|[Schwab, Patrick, Lorenz Linhardt, Stefan Bauer, Joachim M. Buhmann, and Walter Karlen. "Learning Counterfactual Representations for Estimating Individual Dose-Response Curves." arXiv preprint arXiv:1902.00981 (2019).](https://arxiv.org/pdf/1902.00981.pdf)|[Python](https://github.com/d909b/drnet)|

#### Learning Causal Effects with Multi-cause Data
|Name|Paper|Code|
|---|---|---|
|Deconfounder|[Wang, Yixin, and David M. Blei. "The blessings of multiple causes." arXiv preprint arXiv:1805.06826 (2018).](https://arxiv.org/abs/1805.06826)|[Python](https://github.com/blei-lab/deconfounder_tutorial)|
||[Imai, Kosuke, and Zhichao Jiang. "Discussion of "The Blessings of Multiple Causes" by Wang and Blei."](https://imai.fas.harvard.edu/research/files/deconfounder.pdf)|NA|
||[D'Amour, Alexander. "On multi-cause causal inference with unobserved confounding: Counterexamples, impossibility, and alternatives." arXiv preprint arXiv:1902.10286 (2019).](https://arxiv.org/abs/1902.10286)|NA|
||[Ranganath, Rajesh, and Adler Perotte. "Multiple causal inference with latent confounding." arXiv preprint arXiv:1805.08273 (2018).](https://arxiv.org/pdf/1805.08273)|NA|
||[Kong, Dehan, Shu Yang, and Linbo Wang. "Multi-cause causal inference with unmeasured confounding and binary outcome." arXiv preprint arXiv:1907.13323 (2019).](https://arxiv.org/pdf/1907.13323.pdf)|NA|
||[Elizabeth L. Ogburn, Ilya Shpitser, Eric J. Tchetgen Tchetgen "Comment on Blessings of Multiple Causes." arXiv preprint arXiv:1910.05438 (2019)](https://arxiv.org/abs/1910.05438v2?from=timeline)|NA|

#### Transfer Learning for Learning Causal Effects
|Name|Paper|Code|
|---|---|---|
|The Y-learner|[Künzel, Sören R., Bradly C. Stadie, Nikita Vemuri, Varsha Ramakrishnan, Jasjeet S. Sekhon, and Pieter Abbeel. "Transfer Learning for Estimating Causal Effects using Neural Networks." arXiv preprint arXiv:1808.07804 (2018).](https://arxiv.org/pdf/1808.07804.pdf)|NA|

#### Variable Selection/Importance for Learning Causal Effects
|Name|Paper|Code|
|---|---|---|
|Variable importance through targeted causal inference|[The Github Repo "varimpact" by Alan E. Hubbard and Chris J. Kennedy, University of California, Berkeley](https://github.com/ck37/varimpact)|[R](https://github.com/ck37/varimpact)|

#### Instrumental Variables
|Name|Paper|Code|
|---|---|---|
|DeepIV|[Hartford, Jason, Greg Lewis, Kevin Leyton-Brown, and Matt Taddy. "Deep iv: A flexible approach for counterfactual prediction." In International Conference on Machine Learning, pp. 1414-1423. 2017.](http://proceedings.mlr.press/v70/hartford17a/hartford17a.pdf)|[Python](https://github.com/jhartford/DeepIV)|
|PDSLasso|[Achim Ahrens & Christian B. Hansen & Mark E Schaffer, 2018. "PDSLASSO: Stata module for post-selection and post-regularization OLS or IV estimation and inference," Statistical Software Components S458459, Boston College Department of Economics, revised 24 Jan 2019.](https://ideas.repec.org/c/boc/bocode/s458459.html)|[STATA](https://statalasso.github.io/)|

### Non-i.i.d Data

#### Learning Causal Effects from Networked Observational Data
|Name|Paper|Code|
|---|---|---|
|Network Deconfounder|[Guo, Ruocheng, Jundong Li, and Huan Liu. "Learning Individual Causal Effects from Networked Observational Data." WSDM 2020.](https://arxiv.org/abs/1906.03485)|[Python](https://github.com/rguo12/network-deconfounder-wsdm20)|
|Causal Inference with Network Embeddings|[Veitch, Victor, Yixin Wang, and David M. Blei. "Using embeddings to correct for unobserved confounding." arXiv preprint arXiv:1902.04114 (2019).](https://arxiv.org/pdf/1902.04114)|[Python](https://github.com/vveitch/causal-network-embeddings)|


#### Learning Causal Effects under Spillover Effect/Interference
|Name|Paper|Code|
|---|---|---|
|Linked Causal Variational Autoencoder (LCVA)|[Rakesh, Vineeth, Ruocheng Guo, Raha Moraffah, Nitin Agarwal, and Huan Liu. "Linked Causal Variational Autoencoder for Inferring Paired Spillover Effects." CIKM 2018.](http://www.public.asu.edu/~rguo12/CIKM18.pdf)|[Python](https://github.com/rguo12/CIKM18-LCVA)|
|GNN-based Causal Effect Estimators|[Ma, Yunpu, Yuyi Wang, and Volker Tresp. "Causal Inference under Networked Interference." arXiv preprint arXiv:2002.08506 (2020).](https://arxiv.org/pdf/2002.08506.pdf)|NA|
#### Learning Time Varying/Dependent Causal Effects
|Name|Paper|Code|
|---|---|---|
|Time Series Deconfounder|[Bica, Ioana, Ahmed M. Alaa, and Mihaela van der Schaar. "Time Series Deconfounder: Estimating Treatment Effects over Time in the Presence of Hidden Confounders." arXiv preprint arXiv:1902.00450 (2019).](https://arxiv.org/pdf/1902.00450.pdf)|NA|
|Recurrent Marginal Structural Networks|[Lim, Bryan. "Forecasting Treatment Responses Over Time Using Recurrent Marginal Structural Networks." In Advances in Neural Information Processing Systems, pp. 7494-7504. 2018.](http://medianetlab.ee.ucla.edu/papers/nips_rmsn.pdf)|[Python](https://github.com/sjblim/rmsn_nips_2018)|
|Longitudinal Targeted Maximum Likelihood Estimation|[Petersen, Maya, Joshua Schwab, Susan Gruber, Nello Blaser, Michael Schomaker, and Mark van der Laan. "Targeted maximum likelihood estimation for dynamic and static longitudinal marginal structural working models." Journal of causal inference 2, no. 2 (2014): 147-185.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4405134/)|[R](https://github.com/joshuaschwab/ltmle)|

## Connections to Machine Learning
### Recommendation
|Name|Paper|Code|
|---|---|---|
|Unbiased Offline Recommender Learning|[Saito, Yuta, Suguru Yaginuma, Yuta Nishino, Hayato Sakata, and Kazuhide Nakata. "Unbiased Recommender Learning from Missing-Not-At-Random Implicit Feedback." In Proceedings of the 13th International Conference on Web Search and Data Mining, pp. 501-509. ACM, 2020.](https://dl.acm.org/doi/abs/10.1145/3336191.3371783)|[Python](https://github.com/usaito/unbiased-implicit-rec-real)|
|Domain Adversarial Matrix Factorization|[Saito, Yuta. "Offline Recommender Learning Meets Unsupervised Domain Adaptation." arXiv preprint arXiv:	arXiv:1910.07295 (2019).](https://arxiv.org/abs/1910.07295)|NA|
|Doubly Robust Joint Learning|[Wang, Xiaojie, Rui Zhang, Yu Sun, and Jianzhong Qi. "Doubly Robust Joint Learning for Recommendation on Data Missing Not at Random." In International Conference on Machine Learning, pp. 6638-6647. 2019.](http://proceedings.mlr.press/v97/wang19n.html)|NA|
|Top-K Off-policy Correction|[Chen, Minmin, Alex Beutel, Paul Covington, Sagar Jain, Francois Belletti, and Ed H. Chi. "Top-k off-policy correction for a REINFORCE recommender system." In Proceedings of the Twelfth ACM International Conference on Web Search and Data Mining, pp. 456-464. ACM, 2019.](https://arxiv.org/abs/1812.02353)|[Python](https://github.com/awarebayes/RecNN)|
|Causal Embedding for Recommendation|[Bonner, Stephen, and Flavian Vasile. "Causal embeddings for recommendation." In Proceedings of the 12th ACM Conference on Recommender Systems, pp. 104-112. ACM, 2018. (**BEST PAPER**)](https://arxiv.org/pdf/1706.07639)|[Python](https://github.com/criteo-research/CausE)|
|Unbiased Offline Recommender Evaluation|[Yang, Longqi, Yin Cui, Yuan Xuan, Chenyang Wang, Serge Belongie, and Deborah Estrin. "Unbiased offline recommender evaluation for missing-not-at-random implicit feedback." In Proceedings of the 12th ACM Conference on Recommender Systems, pp. 279-287. ACM, 2018.](https://dl.acm.org/citation.cfm?id=3240355)|[Python](https://github.com/ylongqi/unbiased-offline-recommender-evaluation)|
|IPS Estimator|[Schnabel, Tobias, Adith Swaminathan, Ashudeep Singh, Navin Chandak, and Thorsten Joachims. "Recommendations as treatments: Debiasing learning and evaluation." arXiv preprint arXiv:1602.05352 (2016).](http://www.jmlr.org/proceedings/papers/v48/schnabel16.pdf)|[Python](http://www.cs.cornell.edu/~schnabts/mnar/index.html)|
|Deconfounded Recsys|[Wang, Yixin, Dawen Liang, Laurent Charlin, and David M. Blei. "The Deconfounded Recommender: A Causal Inference Approach to Recommendation." arXiv preprint arXiv:1808.06581 (2018).](https://arxiv.org/pdf/1808.06581)|NA|

### Learning to Rank
|Name|Paper|Code|
|---|---|---|
|Heckman^{rank}|[Ovaisi, Zohreh, Ragib Ahsan, Yifan Zhang, Kathryn Vasilaky, and Elena Zheleva. "Correcting for Selection Bias in Learning-to-rank Systems." arXiv preprint arXiv:2001.11358 (2020).](https://arxiv.org/abs/2001.11358)|NA|
|TrustPBM| [Agarwal, Aman, Xuanhui Wang, Cheng Li, Mike Bendersky, and Marc Najork. "Addressing Trust Bias for Unbiased Learning-to-Rank." In The World Wide Web Conference, pp. 4-14. ACM, 2019.](https://research.google/pubs/pub47859/) |NA|
|Unbiased LambdaMart|[Hu, Ziniu, Yang Wang, Qu Peng, and Hang Li. "Unbiased LambdaMART: An Unbiased Pairwise Learning-to-Rank Algorithm." In The World Wide Web Conference, pp. 2830-2836. ACM, 2019.](https://acbull.github.io/pdf/unbias.pdf)|[C++,Python,R](https://github.com/acbull/Unbiased_LambdaMart)|
|Intervention Harvesting|[Agarwal, Aman, Ivan Zaitsev, Xuanhui Wang, Cheng Li, Marc Najork, and Thorsten Joachims. "Estimating Position Bias without Intrusive Interventions." In Proceedings of the Twelfth ACM International Conference on Web Search and Data Mining, pp. 474-482. ACM, 2019.](https://dl.acm.org/doi/10.1145/3289600.3291017)|NA|
|IPW_rank and the Dual Learning Algorithm|[Qingyao Ai, Keping Bi, Cheng Luo, Jiafeng Guo, W. Bruce Croft. 2018. Unbiased Learning to Rank with Unbiased Propensity Estimation. In Proceedings of SIGIR '18](https://arxiv.org/abs/1804.05938)|[Python](https://github.com/QingyaoAi/Unbiased-Learning-to-Rank-with-Unbiased-Propensity-Estimation)|
|Propensity SVM-rank|[Joachims, Thorsten, Adith Swaminathan, and Tobias Schnabel. "Unbiased learning-to-rank with biased feedback." In Proceedings of the Tenth ACM International Conference on Web Search and Data Mining, pp. 781-789. ACM, 2017. (**BEST PAPER**)](https://dl.acm.org/ft_gateway.cfm?id=3018699&type=pdf)|[Python](http://www.cs.cornell.edu/people/tj/svm_light/svm_proprank.html)|
|Regression EM|[Wang, Xuanhui, Nadav Golbandi, Michael Bendersky, Donald Metzler, and Marc Najork. "Position bias estimation for unbiased learning to rank in personal search." In Proceedings of the Eleventh ACM International Conference on Web Search and Data Mining, pp. 610-618. ACM, 2018.](https://pub-tools-public-publication-data.storage.googleapis.com/pdf/3bace79f9bcead0b20dec31e2a0878346ad2fb0d.pdf)|NA|
|Various Bias Models|[Wang, Xuanhui, Michael Bendersky, Donald Metzler, and Marc Najork. "Learning to rank with selection bias in personal search." In Proceedings of the 39th International ACM SIGIR conference on Research and Development in Information Retrieval, pp. 115-124. ACM, 2016.](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45286.pdf)|NA|

### Off-line Policy Evaluation/Optimization
|Name|Paper|Code|
|---|---|---|
|Optimal Kernel Balancing|[Andrew Bennett, Nathan Kallus. "Policy Evaluation with Latent Confounders via Optimal Balance"](http://arxiv.org/abs/1908.01920)|[Python](https://github.com/CausalML/LatentConfounderBalancing)|
|BanditNet|[Joachims, Thorsten, Adith Swaminathan, and Maarten de Rijke. "Deep learning with logged bandit feedback." (2018).](https://openreview.net/pdf?id=SJaP_-xAb)|[Python](https://www.cs.cornell.edu/people/tj/banditnet/index.html)|
|Counterfactual Risk Minimization (POEM)|[Swaminathan, Adith, and Thorsten Joachims. "Counterfactual risk minimization: Learning from logged bandit feedback." In International Conference on Machine Learning, pp. 814-823. 2015.](http://www.jmlr.org/proceedings/papers/v37/swaminathan15.pdf)|[Python](http://www.cs.cornell.edu/~adith/POEM/index.html)|
|Self Normalized Estimator|[Swaminathan, Adith, and Thorsten Joachims. "The self-normalized estimator for counterfactual learning." In Advances in Neural Information Processing Systems, pp. 3231-3239. 2015.](http://papers.nips.cc/paper/5748-the-self-normalized-estimator-for-counterfactual-learning.pdf)|[Python](http://www.cs.cornell.edu/~adith/POEM/index.html)|
|Focused Context Balancing|[Zou, Hao, Kun Kuang, Boqi Chen, Peixuan Chen, and Peng Cui. "Focused Context Balancing for Robust Offline Policy Evaluation." In Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, pp. 696-704. ACM, 2019.](http://delivery.acm.org/10.1145/3340000/3330852/p696-zou.pdf?ip=209.147.139.170&id=3330852&acc=ACTIVE%20SERVICE&key=B63ACEF81C6334F5%2EBD7B0059B564CDBA%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1568671555_f79e8c0ff7c1b351ed2bbc13191485ef)|NA|
|Surrogate Policy|[Xie, Yuan, Boyi Liu, Qiang Liu, Zhaoran Wang, Yuan Zhou, and Jian Peng. "Off-Policy Evaluation and Learning from Logged Bandit Feedback: Error Reduction via Surrogate Policy." arXiv preprint arXiv:1808.00232 (2018).](https://arxiv.org/abs/1808.00232)|NA|
|Balanced Policy Evaluation and Learning|[Kallus, Nathan. "Balanced policy evaluation and learning." In Advances in Neural Information Processing Systems, pp. 8895-8906. 2018.](http://papers.nips.cc/paper/8105-balanced-policy-evaluation-and-learning.pdf)|NA|
|Confounding-robust Policy Learning|[Kallus, Nathan, and Angela Zhou. "Confounding-robust policy improvement." In Advances in Neural Information Processing Systems, pp. 9269-9279. 2018.](http://papers.nips.cc/paper/8105-balanced-policy-evaluation-and-learning)|NA|
|Multi-action Policy Learning|[Zhou, Zhengyuan, Susan Athey, and Stefan Wager. "Offline multi-action policy learning: Generalization and optimization." arXiv preprint arXiv:1810.04778 (2018).](https://arxiv.org/abs/1810.04778)|NA|
|Efficient Policy Learning|[Athey, Susan, and Stefan Wager. "Efficient policy learning." arXiv preprint arXiv:1702.02896 (2017).](https://arxiv.org/abs/1702.02896)|NA|

### Natural Language Processing
|Name|Paper|Code|
|---|---|---|
|Causal Text Embeddings|[Veitch, Victor, Dhanya Sridhar, and David M. Blei. "Using Text Embeddings for Causal Inference." arXiv preprint arXiv:1905.12741 (2019).](https://arxiv.org/pdf/1905.12741.pdf)|[Python](https://github.com/blei-lab/causal-text-embeddings)|
|Handling Missing/Noisy Treatment|[Wood-Doughty, Zach, Ilya Shpitser, and Mark Dredze. "Challenges of Using Text Classifiers for Causal Inference." In Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing, pp. 4586-4598. 2018.](https://aclweb.org/anthology/D18-1488)|[Python](https://github.com/zachwooddoughty/emnlp2018-causal)|
|Conditional Treatment-adversarial Learning Based Matching|[Yao, Liuyi, Sheng Li, Yaliang Li, Hongfei Xue, Jing Gao, and Aidong Zhang. "On the estimation of treatment effect with text covariates." In Proceedings of the 28th International Joint Conference on Artificial Intelligence, pp. 4106-4113. AAAI Press, 2019.](https://pdfs.semanticscholar.org/2e2f/39232771711248940f68c3c1d6bd0a22c3e4.pdf)|NA|
|Causal Inferences Using Texts|[Egami, Naoki, Christian J. Fong, Justin Grimmer, Margaret E. Roberts, and Brandon M. Stewart. "How to make causal inferences using texts." arXiv preprint arXiv:1802.02163 (2018).](https://arxiv.org/pdf/1802.02163.pdf)|NA|
|Causal FS for text classification|[Michael J. Paul. Feature selection as causal inference: experiments with text classification. Conference on Computational Natural Language Learning (CoNLL), Vancouver, Canada. August 2017.](https://www.aclweb.org/anthology/K/K17/K17-1018.pdf)|NA|

### Counterfactual Explanations
|Paper|Code|
|---|---|
|[Mothilal, Ramaravind Kommiya, Amit Sharma, and Chenhao Tan. "Explaining machine learning classifiers through diverse counterfactual explanations." arXiv preprint arXiv:1905.07697 (2019).](https://arxiv.org/pdf/1905.07697.pdf)|[Python](https://github.com/microsoft/DiCE)|
|[Russell, Chris. "Efficient search for diverse coherent explanations." In Proceedings of the Conference on Fairness, Accountability, and Transparency, pp. 20-28. 2019.](https://dl.acm.org/doi/pdf/10.1145/3287560.3287569)|[Python](https://bitbucket.org/ChrisRussell/diverse-coherent-explanations/)|
|[Wachter, Sandra, Brent Mittelstadt, and Chris Russell. "Counterfactual explanations without opening the black box: Automated decisions and the GDPR." Harv. JL & Tech. 31 (2017): 841.](https://heinonline.org/hol-cgi-bin/get_pdf.cgi?handle=hein.journals/hjlt31&section=29)||


### Counterfactual Fairness
|Paper|Code|
|---|---|
|[Kusner, Matt J., Joshua Loftus, Chris Russell, and Ricardo Silva. "Counterfactual fairness." In Advances in Neural Information Processing Systems, pp. 4066-4076. 2017.](http://papers.nips.cc/paper/6995-counterfactual-fairness.pdf)|[Python](https://github.com/mkusner/counterfactual-fairness)|
|[Chiappa, Silvia. "Path-specific counterfactual fairness." In Proceedings of the AAAI Conference on Artificial Intelligence, vol. 33, pp. 7801-7808. 2019.](https://www.aaai.org/ojs/index.php/AAAI/article/download/4777/4655)||
|[Russell, Chris, Matt J. Kusner, Joshua Loftus, and Ricardo Silva. "When worlds collide: integrating different counterfactual assumptions in fairness." In Advances in Neural Information Processing Systems, pp. 6414-6423. 2017.](http://papers.nips.cc/paper/7220-when-worlds-collide-integrating-different-counterfactual-assumptions-in-fairness.pdf)||
|[Garg, Sahaj, Vincent Perot, Nicole Limtiaco, Ankur Taly, Ed H. Chi, and Alex Beutel. "Counterfactual fairness in text classification through robustness." In Proceedings of the 2019 AAAI/ACM Conference on AI, Ethics, and Society, pp. 219-226. 2019.](https://dl.acm.org/doi/pdf/10.1145/3306618.3317950)||

### Reinforcement Learning
|Name|Paper|Code|
|---|---|---|
|Deconfounded RL|[Lu, Chaochao, Bernhard Schölkopf, and José Miguel Hernández-Lobato. "Deconfounding reinforcement learning in observational settings." arXiv preprint arXiv:1812.10576 (2018).](https://arxiv.org/pdf/1812.10576)|[Python](https://github.com/CausalRL/DRL)|
||[Vansteelandt, Stijn, and Marshall Joffe. "Structural nested models and G-estimation: the partially realized promise." Statistical Science 29, no. 4 (2014): 707-731.](https://arxiv.org/pdf/1503.01589.pdf)|NA|
|Counterfactual-Guided Policy Search (CF-GPS)|Buesing, Lars, Theophane Weber, Yori Zwols, Sebastien Racaniere, Arthur Guez, Jean-Baptiste Lespiau, and Nicolas Heess. "Woulda, Coulda, Shoulda: Counterfactually-Guided Policy Search." arXiv preprint arXiv:1811.06272 (2018).|NA|

### Multi-Armed Bandit/Causal Bandit
|Name|Paper|Code|
|---|---|---|
|Causal Bandits|[Lattimore, Finnian, Tor Lattimore, and Mark D. Reid. "Causal bandits: Learning good interventions via causal inference." In Advances in Neural Information Processing Systems, pp. 1181-1189. 2016.](https://arxiv.org/abs/1606.03203)|NA|
|Offline+MAB|[Ye, Li, Yishi Lin, Hong Xie, and John Lui. "Combining Offline Causal Inference and Online Bandit Learning for Data Driven Decisions." arXiv preprint arXiv:2001.05699 (2020).](https://arxiv.org/pdf/2001.05699v1.pdf)|NA|
|B-kl-UCB, B-TS|[Zhang, Junzhe, and Elias Bareinboim. "Transfer learning in multi-armed bandit: a causal approach." In Proceedings of the 16th Conference on Autonomous Agents and MultiAgent Systems, pp. 1778-1780. 2017.](http://www.ifaamas.org/Proceedings/aamas2017/pdfs/p1778.pdf)|NA|
|Incremental Model|[Sawant, Neela, Chitti Babu Namballa, Narayanan Sadagopan, and Houssam Nassif. "Contextual Multi-Armed Bandits for Causal Marketing." arXiv preprint arXiv:1810.01859 (2018).](https://arxiv.org/pdf/1810.01859)|NA|

### Invariant Prediction
|Name|Paper|Code|
|---|---|---|
|Deep Global Balancing Regression|Kuang, Kun, Peng Cui, Susan Athey, Ruoxuan Xiong, and Bo Li. "Stable Prediction across Unknown Environments." In Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, pp. 1617-1626. ACM, 2018.|NA|
|A Simple Algorithm for Invariant Prediction| |[Julia](https://github.com/richardkwo/InvariantCausal.jl)|

### Causality and GAN
|Name|Paper|Code|
|---|---|---|
||Odena, Augustus, Jacob Buckman, Catherine Olsson, Tom B. Brown, Christopher Olah, Colin Raffel, and Ian Goodfellow. "Is Generator Conditioning Causally Related to GAN Performance?." arXiv preprint arXiv:1802.08768 (2018).|NA|
|Causal GAN|Kocaoglu, Murat, Christopher Snyder, Alexandros G. Dimakis, and Sriram Vishwanath. "CausalGAN: Learning Causal Implicit Generative Models with Adversarial Training." arXiv preprint arXiv:1709.02023 (2017).|[Python](https://github.com/mkocaoglu/CausalGAN)|


## Learning Causal Relations
### With i.i.d. Data
|Name|Paper|Code|
|---|---|---|
|IC algorithm| |[Python](https://github.com/akelleh/causality)|
|PC algorithm|P. Spirtes, C. Glymour, and R. Scheines. Causation, Prediction, and Search. The MIT Press, 2nd edition, 2000.|[Python](https://github.com/keiichishima/pcalg) [R](https://github.com/cran/pcalg) [Julia](https://github.com/mschauer/CausalInference.jl)|
|FCI algorithm| |[R](https://github.com/cran/pcalg)|

#### Learning IV
|Name|Paper|Code|
|---|---|---|
|IV Discovery Methods|[Silva, Ricardo, and Shohei Shimizu. "Learning instrumental variables with structural and non-gaussianity assumptions." The Journal of Machine Learning Research 18, no. 1 (2017): 4321-4369.](http://www.jmlr.org/papers/volume18/17-014/17-014.pdf)|NA|

#### Distinguishing Cause from Effect (Bivariate)
|Name|Paper|Code|
|---|---|---|
|BMLiNGAM|S. Shimizu and K. Bollen. Bayesian estimation of causal direction in acyclic structural equation models with individual-specific confounder variables and non-Gaussian distributions. Journal of Machine Learning Research, 15: 2629-2652, 2014.|[Python](https://github.com/taku-y/bmlingam)|

#### Conditional Independence Tests (for Constraint-based Algorithms)
|Name|Paper|Code|
|---|---|---|
|RCIT|   |[R](https://github.com/ericstrobl/RCIT)|

#### Causal Discovery Meets Probabilistic Logic Programming
|Name|Paper|Code|
|---|---|---|
|Causal PSL|Sridhar, Dhanya, Jay Pujara, and Lise Getoor. "Scalable Probabilistic Causal Structure Discovery." In IJCAI, pp. 5112-5118. 2018.|[Java](https://bitbucket.org/linqs/causpsl)|

### Learning Causal Relationships with non-i.i.d. Data


