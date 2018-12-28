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

