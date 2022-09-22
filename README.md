# Object-classification
In this project, we try to classify images of two kinds of objects: fruits and household appliances. Four different computer vision algorithms have been implemented for four different cases. In the first two cases two models were implemented that tries try to classify different classes of home appliances and fruits separately. In the third case a model implemented that tries to classify images into fruit or household objects. In the fourth and last case a model was implemented that tries to classify every sub-class from both fruits and household appliances.
## Dataset
The dataset consist of images of five types of fruits and five types of household appliances. The different types of fruits and household appliance images are presented below:

| Fruits  | Household appliances  | 
| :---: | :---: |
| Apples  | Clocks  |
| Oranges  | Computer Keyboard  |
| Pears  | Lamp  |
| Sweet Peppers  | Telephone  |
| Mushrooms  | Television  |

Εach class for both fruit and household appliances consists of 600 samples. The initial dataset is divided into a train set where our models will be trained, a test set where the evaluation will be done, and a validation set where the validation will be done. All the different datasets are stratified meaning that there are an equal number of classes. Specifically for each class, 450 samples belong to the train set 50 to the test set and 100 to the validation set.

# Model architecture
We used the same model architecture for all cases. Specifically, the model consists of four 2D - convolutional layers of different dimensions with intermediate maxpooling layers. The activation function for the convolutional levels was ReLU. At the end there is a dense layer with dimension 512 followed by the output layer which uses softmax activations as a function. The dimension of the last layer changes depending on the number of classes we have in each case. A dropout layer was added after the last level with a dropout rate of 0.25.

The model was trained in all cases with batch size 64 for 150 epochs. Adam optimizer algorithm was used for back propagation with learning rate 0.005.

# Results case 1 - Classification of fruits:





