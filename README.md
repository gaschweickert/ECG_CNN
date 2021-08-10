# NeuralNet
The neural network project in this repository represents a group effort to develop a CNN capable of classifying pathological heartbeats in ECG signals. The MIT-BIH arrhythmia database was used for this task, it is frequently used in machine learning studies on temporal pattern classification. There were no specification as to what approach should be used to solve this task. Our team settled on a one-dimentsional CNN, with our architecture being inspired by the work of Wu et al. (2021). The end result was a general classifier that could identify 10 different types of arrythmias with ~95% accuracy. To push our investigation futher we also compared training the network on single patients versus a transfer learning version or per patient classification (where the network is first trained on all patients (-1) and then the latter layers are retrained on a single patient). The difference between the two methods was insignificant in the end, this is likely a consequence of the relatively few number of frozen (transfer learning) parameters versus the total number of trainable parameters. For this project I ended up creating the entire training and testing pipeline (from network architecture to hyperparameter tuning), as well as, parts of the data preprocessing pipeline. Our final grade was a 9.5/10.

Wu, M., Lu, Y., Yang, W., and Wong, S. Y.
(2021). A study on arrhythmia via ecg signal
classification using the convolutional neural network. Frontiers in Computational Neuroscience,
14:106.
