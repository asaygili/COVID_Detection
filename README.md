# COVID_Detection

To run the COVID_Detection_GUI

1. MATLAB version 2020a and above must be installed on your computer.
2. The vl_feat library used for feature extraction needs to be extracted from the compressed file and installed. The following code must be run for installation.
run('yourPath\vlfeat-0.9.19\toolbox\vl_setup.m');
3. For vl_feat libraries to work, Microsoft Visual C++ 2008 Service Pack 1 Redistributable Package must be installed.
3. Our trained model "trainedModelsvmcubic985.mat" file (https://disk.yandex.com.tr/d/7Q5k2hhZ7OBEsQ for download), segment_em_gmm.m file for segmentation process with EM based GMM model and our GUI file "COVID_Detection_app. mlapp" files must be in the same directory.
4. After all these processes, App Designer should be opened in MATLAB application and GUI file should be selected by saying open.
5. After opening the GUI in App Designer, it is enough to press the Run button. The GUI will then open and you will be prompted to select an image.
6. The application is modeled only with CT images. Therefore, by selecting a COVID positive or negative CT image, you can see the program segment and generate Test Result for you. In practice, training and testing processes were carried out using the following data set.
https://www.kaggle.com/plameneduardo/sarscov2-ctscan-dataset
