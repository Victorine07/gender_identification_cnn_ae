# gender_identification and age estimation

### Experiments

#### Datasets:

1. We used celebA dataset for gender identification only
2. We used Audience dataset for gender identification along with age estimation for classes being ranges of age
3. We used UTKFace dataset for gender identification along with age estimation for one age representing a class

#### Methods:

1. for gender identification only, we used the following networks:
I. 

      a. VGG16 : maximum of 98% accuracy on the test set and 97.89% accuracy on the training set
      b. VGG19 : maximum of 97.7% accuracy on the test set and 97.51% accuracy on the training set
      c. ResNet18 : maximum of 96.32% accuracy on the test set and 97.01% accuracy on the training set

2. for the gender identification with age estimation, we used the following networks based on VGGFace:
I.

      a. VGGFACE based on resnet 50 with UTKFace dataset: 
            maximum accuracy of 91.2% on the test set and 90.85% on the training set for the gender identification only and 18.5% on the test set and 17.65% on the training set for the age estimation
      b. VGGFACE based on VGG16 with Adience dataset: 
            maximum accuracy of 91.6% on the test set and 90.95% on the training set for the gender identification only and 55.4% on the test set and 54.8% on the training set for the age estimation
 
### Other
We noticed that cropping differently the images might improve the performance, especially for the age estimation but this takes time. Also, increasing the training set size can improve the performance, as our training used less than 20k images for all the networks. At last, it is also important to know if the dataset is correctly labbelled to really know if the model performs well or not. Let's note that, the model cannot account for individuals that do not identify theirselves with a specific gender, and this is one limitation on gender identification


