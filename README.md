

# MinimaxTree

**Content**
This is the code repository for the research publication "Minimax Decision Trees via Martingale Approximations" by Zhenyuan Zhang and Hengrui Luo. 
The manuscript of this paper can be accessed at [https://arxiv.org/pdf/2502.16758](https://arxiv.org/abs/2502.16758). 

 - We provided a set of working code of simulation and computation of the decision tree regression via minimax martingale splitting criterion.
 -  Reproducible Code
	 - in Single_depth.ipynb, we provide the single minimax tree (using minimax martingale splitting criterion) as proposed in the paper, and reproduced the synthetic experiments using the synthetic function with different max_depths and comparison against different other decision tree regression methods (e.g., L1, variance).
	 - in Single_mix.ipynb, we provide the single-run and multiple-run code for the layer-wise splitting strategies as proposed in the paper, and reproduced the synthetic experiments using the synthetic function. We introduced cylic minimax to handle higher dimensional input predictor problems.
	 - in Global.ipynb, we provide the code that generates comparison of the optimal tree, Scikit-learn DecisionTreeRegressor, our MinimaxSplit tree, and VarianceSplit tree on a sinusoidal target function.
     - in Forest.ipynb, we provide the code that generates comparison of the ensemble methods proposed to accomondate the minimax martingale design.
     - in Astr.ipynb, we provide the code that reproduces our result on astronaut sample images shown in our paper.

**Abstract**
We develop a martingale-based approach to constructing decision trees that efficiently approximate a target variable through recursive conditioning. We introduce MinimaxSplit, a novel splitting criterion that minimizes the worst-case variance at each step, and analyze its cyclic variant, proving an exponential error decay rate under mild conditions. Our analysis builds upon partition-based martingale approximations, providing new insights into their convergence behavior. Unlike traditional variance-based methods, MinimaxSplit avoids end-cut preference and performs well in noisy settings. We derive empirical risk bounds and also explore its integration into random forests.

**Citation**
We provided both iPynb illustrative code, Python production code for reproducible and experimental purposes under [LICENSE](https://github.com/hrluo/MinimaxTree/blob/master/LICENSE).
Please cite our paper using following BibTeX item:

    @article{zl2025minimax,
		title={Minimax Decision Trees via Martingale Approximations}, 
		author={Zhenyuan Zhang and Hengrui Luo},
		year={2025}, 
		eprint={2502.16758},
		archivePrefix={arXiv},
		primaryClass={math.ST},
		url={https://arxiv.org/abs/2502.16758}, 
    }

Thank you again for the interest and please reach out if you have further questions.
