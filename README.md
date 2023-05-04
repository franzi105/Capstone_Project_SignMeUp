
# SignMeUp: Real-time recognition of American Sign Language

This project aims to develop a machine learning model that recognizes American Sign Language (ASL) signs in videos. The model is designed to be integrated into an innovative learning app that enables users to practice ASL signs using their phone camera and receive instant feedback. This makes learning ASL more accessible, particularly for the hearing parents of deaf children who may not be familiar with ASL.
![image](./images/SignMeUp_Logo.png)
# Setup and Installation

To install and run this project, follow these steps:

1. Clone this repository to your local machine.

2. Setup virtual environment and install the required libraries:

```python
pyenv local 3.9.8
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

3. Download the dataset from [Isolated Sign Recognition Language/Data](https://www.kaggle.com/competitions/asl-signs/data) and save it in the `data` folder.

Note: This project is a Kaggle competition, and therefore requires a Kaggle account to download the dataset. You will need to accept the competition rules and agree to the terms and conditions before you can access the dataset.

# Notebooks Overview
* Domain Knowledge and information about the project : 
  * "01_DomainKnowledge"
  * this notebook gives first insights into the project and performs EDA on the whole dataset including visualization of video sequences
* EDA of the dataset:
  * "02_EDA"
* Visualization of sign language sequences:
  * "03.1_Visualization"
* Drawing landmarks on video files: 
  * "03.2_DrawMediaPipe_fromVideoFile"
  * load a mp4 video file to the notebook to detect MediaPipe landmarks and draw detected markers on the video. 
* Dummy Classifier as zero baseline model:
  * "04.1_Dummy_Baseline"
* SKTime Baseline models:
  * "04.2_SKTIME_first_baseline_model"
* Preprocessing Notebook: 
  * "05_Preprocessing"
  * Notebook to preprocess raw data and compile all sequences into one dataset 
* Modeling: 
  * "06.1_Modeling_LSTM"
  * "06.2_Modelling_Rocket"
  * "06.3_Modelling_sklearn"
* Real Time prediction: 
  * "07_Real-Time-Demo_SignMeUp"
  * further explained in 'Usage'

# Usage 

Steps to Use ASL Recognition Model for real time prediction:

1. Start the ASL real time prediction by running the notebook "07_Real-Time-Demo_SignMeUp".
2. Ensure that you have good lighting conditions and a clear view of your hand gestures for best results.

### Game Menu
![image](./images/Real-Time-Demo-Menu.png)
### Note:

- Make sure that the sign is in the dataset used to train the model for accurate recognition.
- If you face any issues with the recognition, try adjusting the lighting or the angle of the camera to get a clearer view of the sign.



# Conclusion

The ASL recognition model developed in this project has the potential to make a significant impact in improving accessibility and communication for the deaf and hard-of-hearing communities. The integration of this model into an innovative learning app has the potential to transform the way people learn ASL, particularly for the hearing parents of deaf children who may not be familiar with ASL.

The next steps for the project involve deploying the model in a mobile application, specifically a sign language learning app. 
Moreover, one of our aim is to collect and add more signs. Additionally, we plan to train models for other sign languages and develop a translation tool that enables natural social interactions and solves everyday problems in public, educational, and commercial settings, such as at a hairdresser or supermarket. The potential impact of these future applications is considerable, making this an exciting and promising project for the advancement of sign language recognition technology.











