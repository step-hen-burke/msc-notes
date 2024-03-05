Title:  Deep Learning Compression for Resource-Constrained Environments
Topic area: Investigate and implement compression techniques to enable the use of deep learning models under resource-constraints

Overview:
Deep learning models are widely applicable in many domains, but can require significant resources to store and perform inference with, which limits their use in certain environments such as mobile devices and IoT devices. This project seeks to explore the constraints and resource considerations that deep learning models are subject to, such as limited memory, processing power, energy consumption, cloud storage costs, model artifact I/O time, etc., and how these constraints can be alleviated in order to save costs associated with machine learning inference and broaden the scenarios in which deep learning models can be applied. 

Research Objectives:
- Identify and compare current approaches to deep neural network compression, taking note of the impact of different network architectures on the applicability and effectiveness of different approaches. Classify approaches by the overarching technique, and based on the resource constraints they can help address: memory, speed, etc.
- Identify typical scenarios within which a deep neural network would be subject to resource constraints, acceptable performance/resource trade-offs, and typical speed and footprint benchmarks that a compressed model should be evaluated against (through interview with industry experts, for example). Additionally, identify any use-cases which are enabled or enhanced by the compression of deployed models. 
- Using standard datasets (MNIST, CIFAR, Treebank, for example. Or others as deemed relevant) and architectures, evaluate the effectiveness of compression techniques in terms of: disk size reduction, memory usage, predictive performance preserved, inference speed, etc. - particularly with regard to important metrics and consumer hardware benchmarks such as typical mobile or IoT hardware.
- Create compressed predictive models for use in resource-constrained environments using combinations of techniques which are deemed to be optimal. Optimal in this context would involve trade-offs between factors explored in RO 3 - model size, inference speed, predictive accuracy, etc. Identify viable compression strategies utilising combinations of previously explored techniques.
- Develop a suite of tools to compress models using combinations of techniques subject to specific resource constraints or target hardware configurations.

Domain Area - Machine Learning (Deep Learning) compression
Problem Area - Resource-constrained deep learning model deployment
