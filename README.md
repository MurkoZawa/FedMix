# FedMix
FedMix is an innovative framework that leverages federated learning techniques to enhance the segmentation of cellular nuclei in histopathological images. By employing a federated approach, FedMix enables multiple clients to collaboratively train machine learning models without sharing their raw data, thus preserving privacy and security. This method is particularly beneficial in medical applications, where data sensitivity is paramount.

Federated learning (FL) is a decentralized machine learning paradigm that allows models to be trained across multiple devices or servers holding local data samples. Instead of transferring data to a central server, FL enables the computation of model updates locally and aggregates these updates to form a global model. This approach not only enhances privacy but also reduces latency and bandwidth consumption.
The clients share model updates with a central server, which aggregates them to improve the global model, without data sharing.
This repository provides an implementation of various federated learning techniques, including:

- FedAvg: A foundational federated averaging algorithm that allows for the training of a global model by aggregating updates from multiple clients.
- FedMix: An advanced approach that enhances the training process by incorporating multiple clients simultaneously.
- FedST: A technique designed to improve model performance by leveraging statistical methods within the federated learning framework.
- FedRGD: An implementation of randomized gradient descent tailored for federated settings, promoting efficient convergence in model training.
- Local Learning: Techniques that focus on optimizing model performance by utilizing local data characteristics, ensuring accurate segmentation of cellular nuclei in histopathological images.
Both FedAvg and FedMix also support incremental learning, enabling models to adapt to new data.

To run the experiments: 

**Optional**: Open the Data_Augmentation notebook and augment the data (in the data folder, there already are the augmented images and labels) and run the cell. If you do that, make sure to move them on the imagesTrAug and labelsTrBW folders.
- Open the notebook of the federated or local learning methodology you want to use, and run all the cells.
- Once you trained your model, test it and calculate the performance measures by running all the cells in the metrics_calculator notebook.
