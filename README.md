# CNN_TransferLearning_Mammal_Classification


The problem statement constituted the requirement to classify images of cats, dogs, horses and horse-riders. We had 25 images of each of the aforementioned categories and we need to train a model that could automatically classify them.

The biggest problem was the availability of so few training examples. When a CNN model was trained from the scratch the accuracy achieved was very less ~ 60%.
Then we tried transfer learning by leveraging the Resnet models trained on imagenet dataset.

We achieved accuracies of 90% without any finetuning. We improved the accuracy to 95% with addition and subsequent finetuning of just 2 custome dense layers introduced after the ResNet base layer.

The model was then tested on a couple of unseen dog images, which was correcly predicted.

Then an experiment was done on a human image that the model has never seen. The human images the model has seen is that of horse riders in their horse riding attires. An image of a human in office along with his computers was parsed and the prediction turned out to be accurate which shows that the model has learnt the features of the objects very well. 

Next a cropped image of a man's hands alongwith a computer was parsed through the model. Extra-ordinarily this image was also predicted correctly.
