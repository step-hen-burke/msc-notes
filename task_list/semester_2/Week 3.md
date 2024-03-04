RO draft:

- Identify and compare current approaches to deep neural network compression, taking note of the impact of different network architectures on the applicability and effectiveness of approaches. 
- Interview industry experts in order to identify typical scenarios within which a deep neural network would be subject to resource constraints, acceptable performance/resource trade-offs, and typical speed and footprint benchmarks that a compressed model should be evaluated against.
- Using standard datasets (MNIST, CIFAR, Treebank, for example. Or others as deemed relevant) evaluate the effectiveness of compression techniques in terms of: disk size reduction, memory usage, predictive performance preserved, inference speed, etc. - particularly with regard to important metrics and consumer hardware benchmarks as identified by industry experts.
- Create compressed predictive models for use in resource-constrained environments using combinations of previously identified techniques which are deemed to be optimal.

Research Domain - Machine Learning (Deep Learning).
Problem Domain - Deploying deep neural networks in resource-constrained environments.


- Identify techniques to identify important and unimportant substructures within networks for the purposes of pruning. These may come from areas such as graph analysis, network analysis, etc. If it is discovered that these techniques may be applied to DNNs, evaluate the performance of models with unimportant substructures removed.