In this assignment we trained and evaluated three different CNN architectures on CIFAR10: 
1) CIFAR10_lenet: a simple LeNet5
2) CIFAR10_model1: LeNet5 + BatchNorm
3) CIFAR10_model2. LeNet5 + BatchNorm + Dropout

We designed 2 variations of the LeNet5 architecture, designed to improve performance. 
We use early stopping, learning rate scheduling, pretraining, saving and transfering weights and data augmentation.
CIFAR10_model2 had the best results in our runs.
Next, we use CIFAR100's 20 superclasses to train the best architecture from scratch (CIFAR100_model).
Then we transfer CIFAR100_model weights to a new model which is then trained on CIFAR10 (CIFAR10_pretrained).
Finally, we evaluate the best models on CIFAR10's test data.  

We provide the weights of all the trained models after the last epoch of training.
The train_model() function implements the training procedure and outputs the resulting the loss and accuracy plots,
as well as a plot of the learning rate per epoch. 

