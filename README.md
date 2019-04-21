# Flipkart_grid_challenge
This is the approach which I used in the Flipkart Grid Challenge 2018 (Round 3). The model is based on VGG 16 with some implementation changes. The implementation is done in Tensorflow.
In order to run this code:
# Preparing dataset to train the model
1. Resize images to 64 x 64 with changing their box information apprpriately.
2. Keep them in a directory and specify the directory name in the configuring_dataset.ipynb file.

# Training and testing the model
1. Run parts of localization_model.ipynb file.
2. You can directly load the dataset into X_train and X_test by using the GeneratedDataset.pickle file.
3. Training will take about 25 minutes on google colab gpu for 50 iterations. However best results are achieved at about 150 itertions. After that the model begins to overfit.
4. After training test it on the testing images (code provided).
