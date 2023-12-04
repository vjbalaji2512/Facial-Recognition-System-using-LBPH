In the context of face recognition, the process involves two fundamental tasks:

## Face Detection:

Objective: Identify the presence of a face in an image.
Techniques: Various methods exist, including Haar Classifier, which will be our chosen approach for face detection.

## Face Recognition:

Objective: Determine the identity of the detected face.
Techniques: Multiple face recognition techniques are available, such as Eigen Faces, Fisher Faces, Local Binary Patterns Histograms (LBPH), and neural networks.
For this project, we have selected Haar Classifier for face detection and LBPH for face recognition.
For a more in-depth understanding of how Haar Classifier and LBPH work, refer to the following [documentation](https://docs.opencv.org/2.4/modules/contrib/doc/facerec/facerec_tutorial.html#local-binary-patterns-histograms)

We are going to divide the entire process into 4 parts:

* Data Preparation - Storing the images of each person in separate folder and label them
* Face Detection - Running Haar Classifier on each image and detect face.
* Training LBPH Face recognizer - Training the recognizer on stored data
* Prediction - check if the face recognizer predicts correctly on test images
