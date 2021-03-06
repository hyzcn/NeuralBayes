### This is the codebase for the paper [Neural Bayes: A Generic Parameterization Method for Unsupervised Representation Learning](https://arxiv.org/abs/2002.09046).

The paper proposes a simple parameterization method called Neural Bayes which allows computing statistical quantities that are in general difficult to compute and opens avenues for formulating new objectives for unsupervised representation learning. Specifically, given an observed random variable x and a latent discrete variable z, we can express p(x|z), p(z|x) and p(z) in closed form in terms of a neural network using our parameterization without restricting the class of these distributions. To demonstrate its usefulness, we develop two independent use cases for this parameterization:

1. Mutual Information Maximization (**MIM**): MIM has become a popular means for self-supervised representation learning. Neural Bayes allows us to compute mutual information between observed random variables x and latent discrete random variables z in closed form. We use this for learning image representations and show its usefulness on downstream classification tasks.

2. Disjoint Manifold Labeling (**DML**): Neural Bayes allows us to formulate an objective which can optimally label samples from disjoint manifolds present in the support of a continuous distribution. This can be seen as a specific form of clustering where each disjoint manifold in the support is a separate cluster. We design clustering tasks that obey this formulation and empirically show that the model optimally labels the disjoint manifolds.


### Citation

If you use this in your work, please cite

```
@article{arpit2020neuralbayes,
  title={Neural Bayes: A Generic Parameterization Method for Unsupervised Representation Learning},
  author={Devansh Arpit, Huan Wang, Caiming Xiong, Richard Socher, Yoshua Bengio},
  journal={arXiv preprint arXiv:2002.09046},
  year={2020}
}
```
