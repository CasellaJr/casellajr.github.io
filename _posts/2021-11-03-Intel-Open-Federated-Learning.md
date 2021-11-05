My PhD course started. The first experiments I will do are about the new Intel Framework for Federated Learning: Intel OpenFL. Link: https://github.com/intel/openfl
Open Federated Learning (OpenFL) is a Python 3 project developed by Intel Labs and Intel Internet of Things Group. It enables organizations to collaborately train a model without sharing sensitive information with each other.

There are basically two components in the library: the collaborator which uses local dataset to train a global model and the aggregator which receives model updates from collaborators and combines them to form the global model.

The aggregator is framework-agnostic, while the collaborator can use any deep learning frameworks, such as Tensorflow or PyTorch.
