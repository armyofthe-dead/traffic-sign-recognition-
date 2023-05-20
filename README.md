**Traffic Sign Recognition Application**

This repository contains code for a Traffic Sign Recognition application. The application uses deep learning techniques to classify traffic signs based on images.

**Dependencies**

Make sure you have the following dependencies installed:

numpy

pandas

matplotlib

cv2

tensorflow

PIL

os

sklearn

keras

tkinter

**You can install the dependencies using the following command:**

pip install numpy pandas matplotlib opencv-python tensorflow pillow scikit-learn keras


**Dataset**

The application uses the German Traffic Sign Recognition Benchmark (GTSRB) dataset. The dataset contains 43 classes of traffic signs.


Download the dataset and extract it to a directory. Set the path to the training data directory in the code

path = os.path.join(cur_path, 'path_to_training_data_directory', str(i))

***Training the Model***

The code trains a Convolutional Neural Network (CNN) model on the traffic sign dataset.

The model architecture consists of several convolutional layers, max pooling layers, dropout layers, and fully connected layers.

To train the model, run the code. The trained model will be saved as my_model.h5.

**Testing the Model**

The code includes a section for testing the accuracy of the trained model on a separate test dataset. The test dataset should be in CSV format, with the "ClassId" and "Path" columns specifying the labels and file paths of the test images, respectively.

Set the path to the test dataset CSV file in the code:

y_test = pd.read_csv('path_to_test_dataset.csv')

To test the accuracy of the model, run the code. The accuracy score will be printed.

**Running the GUI Application**

The code includes a graphical user interface (GUI) application for traffic sign recognition. It allows you to upload an image and recognize the traffic sign present in the image.

To run the GUI application, execute the code. A window will open, and you can click the "Upload an image" button to select an image for classification. The predicted traffic sign label will be displayed.

Note: You need to provide the path to the trained model file (.h5) in the code:

model = load_model('path_to_trained_model.h5')

the file for model is model.py  and file for GUI is graphic.py

