# tumour-classifier
For our IT1244 Project, we devised a VGG16-ANN model that accurately classifies the tumour as benign or malignant based on MRI images.

**Description**

In recent years, there has been growing interest in developing Convolutional Neural Network (CNN) machine learning models that can accurately classify MRI scans of brain tumours into benign or malignant. Our project aims to create a model that can accurately perform this binary classification task. Moreover, to unveil the black-box nature of most neural network models, we have decided to use GradCAM to explain what feature of the image contributed to the output by each model. Since our dataset was limited (231 images) and mildly imbalanced (62 benign: 129 malignant), we also explored different ways to augment our training data to ensure our trained model is more robust and flexible.

**Workflow**
1. Data preparation which consists of two steps: Preprocessing and Augmentation
2. Creating and fine-tuning hyperparameters for the three models: Baseline CNN model, VGG16-ANN model with varied number of VGG16 layers frozen and VGG16-PCA-XGBoost
3. Plotting of performance graphs with various metrics used
4. Use GradCAM to understand the inner workings of each model
#Note: GradCAM was not able to be used for VGG16-XGBoost (reason as stated in report)

**Getting Started**
1. Dependencies: keras version 2.15.0
2. Ensure file paths to dataset are correct: The first code block specifies the file path to the dataset. If the dataset folder is moved to a different location please specify the new file path to ensure that the program can find the dataset. If the unzipped folder is used without modification then the default file path given will work fine.
3. Installation of necessary packages: The second code block contains all the import statements

'''

!pip install numpy==1.24.3

##remaining import statements...

!pip install tensorflow==2.12.1

'''

Remove the triple backticks (') at the top and the bottom of the code block to run the code which installs all the necessary packages. If all packages are already installed you can reapply the triple backticks to prevent packages from being installed again.

**Executing the program**
The code code blocks should be run in order. The function of each code block is documented neatly. An alternative is to click the tab "runtime" -> "runall" to run all the blocks of code in order. There is also a table of contents that can be accessed by clicking the table of contents icon at the top left of the page.

**Authors**
Justin Tan Min Shi (A0217325L)
Han Yong Yi Jace (A0221948Y)
Sng Zhi Wen Collin (A0252248E)
Ryan Justyn (A0276053E)
