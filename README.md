# SeeFood: a food detection object detection framework built on Darknet's YOLO Algorithm for Deep Learning.

## Food100 YOLO Training Tools
The following instructions concentrated on describing YOLO v2 setup and training.
To get DarkNet YOLO training to work, we needs

* Object bounding box file for each image
* Class name file for all the category names
* Training dataset file for the list of training images
* Validating dataset file for the list of validating images
* Configuration file for YOLO neural network specification
* Data location file for finding all the data information

## Data
Food100 dataset [UEC FOOD 100](http://foodcam.mobi/dataset100.html),
it requires post processing to make bounding box that fit into DarkNet's YOLO training requirements.

## Algorithm     
SeeFood is a food identification algorithm, which when provided with an image containing food item(s), provides you with information on that item. The algorithm works as follows on the high-level:    

* It creates bounding boxes around “supposed” food items which it recognizes
* This information is then passed to a neural network with pre-calculated weights
* After many thousands of iterations, the algorithm converges to a sort of “stable” state after which we don’t see a lot of improvement in performance
* At this stage, the algorithm successfully recognizes most if not all food items in the image.    

SeeFood is a supervised learning model which calculates the probability that the food in the image belongs to a particular class and returns the class with the maximum probability.  

