# YogaPoseDetection

In this project, we leverage transfer learning models in PyTorch and TensorFlow to classify between similar yoga pose images.

There are four poses: Dolphin, Downward facing dog, Sphinx, and Upward facing dog. 
The first two poses are very similar, and the latter two poses are also similar. 
The only difference in each pair is the angle of the arms. 

We compare the performance of transfer learning models with that of from-scratch neural network models, and examine
the advantages and drawbacks of different approaches. Various models (Resnet18, Resnet50, InceptionV3, InceptionResnetV2, Custom built models), optimizers (SGD and Adam), number of trainable layers, and loss functions (Categorical cross entorpy and SVM Multi marginal loss) were explored. 

We confirm that ResNet does not work well on Tensorflow keras as mentioned in the article
https://l7.curtisnorthcutt.com/towards-reproducibility-benchmarking-keras-pytorch. 

See the [accuracy summary.](https://github.com/euniceky/YogaPoseDetection/blob/master/AccuracySummary.pdf) The best model was ResNet18 in PyTorch which has accuracy 92.31%. 

