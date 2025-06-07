# CS5720_Home_Assignment_2
**Student Name:** Trang Horn

**Student ID:** 700683454
## Question 1: Convolution Operations with Different Parameters
### Task: Implement Convolution with Different Stride and Padding
**Description/Explanation:**
This script demonstrated how 2D convolution behaves with different strides and padding configurations using TensorFlow. The script used NumPy and Tensor Flow/keras to perform convolution on a 5x5 input matrix using a 3x3 kernel. The resulting features are printed for four cases:
- Strides 1 with VALID padding
- Stride 1 with SAME padding
- Stride 2 with VALID padding
- Stride 2 with SAME padding 

## Question 2: CNN Feature Extraction with Filters and Pooling
### Task 1: Implement Edge Detection Using Convolution
**Description/Explanation:**
This script applies Sobel X and Sobel Y filters to a grayscale image using OpenCV(cv2) to detect edges on an image in the x-direction and y-direction. It reads an image from a URL, applied the filters, and display the original and filtered results using Matplotlib. 

**Image Source:**
https://raw.githubusercontent.com/scikit-image/scikit-image/main/skimage/data/camera.png

### Task 2: Implement Max Pooling and Average Pooling
**Description/Explanation:**
This script illustrates max pooling and average pooling on a randomly generated 4x4 image matrix using TensorFlow/Keras. It outputs the original matrix, max pooled matrix, and average pooled matrix, which demonstrate how pooling reduces spatial dimensions.

## Question 3: Data Processing - Standardization vs. Normalization
### Task: Explore standardization and normalization techniques on a dataset and analyze their impact
**Description/Explanation:**
This code compared the impact of Min-Max Normalization and Z-score standardization on the Iris dataset, printed out the transformed datasets, and compared them by visualizing distributions using histograms. It then trains Logistic Regression models on raw data and scaled data, and then compares their classification accuracy. The output of the script includes transformed datasets, histogram visualization of distributions, and accuracy across preprocessing methods.

**Questions to Answer:**
- Standardization (Z-score Normalization): Rescales data to have zero mean (0) and unit variance (1). It works well when data has outliers, as it preserves relative variations, and it is useful when data follow a Gaussian (normal) distribution. It is used in statistical models such as PCA, SVM, Logistic Regression, and ECG Analysis, where data is expected to be normally distributed.
- Normalization (Min-Max Scaling): Rescales data to a fixed range [0, 1]. It is sensitive to outliers, which means that if one value is extremely high, it skews all the data.  It also loses variance information, making extreme values less distinguishable. It is used in deep learning models such as CNNs, RNNs, LSTMs, and ECG classifications, where inputs must be in a fixed range.
