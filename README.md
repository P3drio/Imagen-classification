# Imagen-classification
This project demonstrates my skills and proficiency in image classification using deep learning techniques. The goal of this project is to classify garbage images with high accuracy. The code provided here showcases the implementation of a ResNet50 model using PyTorch and the torchvision library.

##Code Structure
The code can be divided into the following sections:

Importing Dependencies: The necessary libraries and modules are imported, including torch, torchvision, and matplotlib.

Data Preparation: The code includes steps to mount Google Drive, install the Kaggle package, and upload the dataset. It also splits the data into training, validation, and testing sets using random_split.

Data Loading: DataLoaders are created for the training and validation sets using DataLoader from torch.utils.data. The show_batch function is provided to visualize a batch of images.

Model Architecture: The ResNet50 model is used for image classification. The model is defined as a subclass of ImageClassificationBase, which includes training and validation step methods. The model's forward method applies a sigmoid activation to the output.

Device Selection: The code selects the appropriate device (GPU if available, else CPU) and moves the model and data to the chosen device using the to_device function and DeviceDataLoader class.

Model Training: The fit function is defined to train the model. It iterates over the training DataLoader, computes the loss, performs backpropagation, and updates the model's parameters. The evaluate function calculates the validation loss and accuracy. The training loop runs for a specified number of epochs.

Model Evaluation: After training, the model is evaluated on the validation dataset, and the results are displayed, including the loss and accuracy for each epoch. The plot_accuracies and plot_losses functions visualize the accuracy and loss curves.

Image Prediction: The predict_image function is provided to make predictions on individual images. An example of a test image prediction is shown, where an image from the test dataset is randomly selected, displayed, and labeled using the trained model.

##Results
The model achieved an accuracy of over 90% on the test dataset. It performed well on test images and correctly classified garbage items. You can experiment with additional images to further test the model's performance.

Feel free to explore and modify the code to enhance the model or try it with your own dataset.

For any questions or inquiries, please contact me at [email address].
