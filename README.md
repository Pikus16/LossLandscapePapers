# LossLandscapePapers
Repo with papers about loss landscape and related topics
 
* Learning Neural Network Subspaces [2021] - https://arxiv.org/abs/2102.10472
  *  In one training run (so with the same computation cost of training 1 model) train a line, curve, or simplex (k-dimensional triangle) of neural networks.
  
  ![image](https://user-images.githubusercontent.com/12414995/124765126-ac16bf80-df03-11eb-8374-4fb249708d99.png)
  *  
  *  Ties into underspecification by showing different models along the line perform differently on downstream tasks.
* Linear Mode Connectivity and the Lottery Ticket Hypothesis [2020] - https://arxiv.org/abs/1912.05671
  * Studies whether networks optimize to same linearly connected minimum (or basin) under different samples of SGD noise (random data order and augmentation). Finds that if two networks share the same SGD noise for a few epochs, then they stay in the same loss basin (for large, non-MNIST problems). Use this to study iterative magnitude pruning (IMP) and find that subnetworks only reach full accuracy when stable to SGD noise.
* Deep ensembles: A loss landscape perspective [2019] - https://arxiv.org/abs/1912.02757
  * Find that deep ensembles outperform bayesian ensembling because different networks are in different loss basins. Find that two of the exact same models, trained starting from different initialization are in different loss basins, and as a consequence, even though they get the same accuracy, often have disagreement between the two (ex: one model is much better at classifying cats, and the other is better for dogs). Cosine similarity between the weight vectors of these networks is approximately 0.
  * Ties into underspecification from this paper (https://arxiv.org/abs/2011.03395) and transfer learning comparisons from this paper (https://arxiv.org/abs/2008.11687)
* Essentially No Barriers in Neural Network Energy Landscape [2018] - https://arxiv.org/abs/1803.00885
  * Finds flat path from minima of two networks 
* Loss Surfaces, Mode Connectivity, and Fast Ensembling of DNNs [2018] https://arxiv.org/abs/1802.10026 
  * Similar to above, shows that loss landscape is connected by simple curve over which train / test accuracy is constant 
* Entropy-SGD optimizes the prior of a PAC-Bayes bound: Generalization properties of Entropy-SGD and data-dependent priors [2018] -
 https://arxiv.org/abs/1712.09376
  *  Less sharp solution in basin is associated with better generalization
* Averaging weights leads to wider optima and better generalization [2018] -https://arxiv.org/abs/1803.05407
  * simple averaging of multiple points along the trajectory of SGD, with a cyclical or constant learning rate, leads to better generalization than conventional training
  * accuracy is higher at the middle of the basin than at the periphery
  
* Visualizing the Loss Landscape of Neural Nets [2017] - https://arxiv.org/abs/1712.09913
