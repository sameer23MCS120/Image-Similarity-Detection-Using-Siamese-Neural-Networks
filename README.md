#About The Project
The Siamese Neural Network for image similarity detection works by processing pairs of images through twin subnetworks that share identical parameters and weights. Each image is passed through convolutional layers within its respective subnetwork to extract feature vectors, which represent the essential characteristics of the images. These feature vectors are then compared using a distance metric, such as Euclidean distance, to measure similarity; smaller distances indicate higher similarity. During training, a contrastive loss function is used to minimize the distance between similar image pairs and maximize the distance between dissimilar ones, enabling the network to learn effectively. The model is trained on a labeled dataset with similar and dissimilar image pairs, optimizing weights through iterative training and backpropagation. Performance is evaluated and optimized using various metrics, and the final model is incorporated into a user-friendly application for practical applications like duplicate image detection and visual search.
#Tools Used
Keras,Jupyter,TensorFlow,Numpy,OpenCv.
#Dataset Used
LABELLED Faces Wild Dataset,sport Celeb.
