# YogaPoseDetection

In this project, we leverage transfer learning models in PyTorch and TensorFlow to classify between similar yoga pose images.

There are four poses: Dolphin, Downward facing dog, Sphinx, and Upward facing dog. 
The first two poses are very similar, and the latter two poses are also similar. 
The only difference in each pair is the angle of the arms. 

We compare the performance of transfer learning models with that of from-scratch neural network models, and examined
the advantages and drawbacks of different approaches. Various models(Resnet18, Resnet50, InceptionV3, InceptionResnetV2) and optimizers (SGD and Adam), and loss functions (Categorical cross entorpy and SVM Multi marginal loss) were tested. 

We confirm that ResNet does not work well on Tensorflow keras as mentioned in the article
https://l7.curtisnorthcutt.com/towards-reproducibility-benchmarking-keras-pytorch. 

