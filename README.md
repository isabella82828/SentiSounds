# 🎶 SentiSounds: Emotion Detection from Speech"
## Project Overview 
This project aims to develop a machine learning model capable of detecting emotions from speech, enhancing personalization in various applications. By analyzing vocal expressions, the model can infer emotional states. 

## Datasets
📂 Two primary datasets were used: 
1. RAVDESS: Comprising approximately 1,500 audio files from 24 actors
2. SAVEE: Containing around 500 audio files from four male actors

## Audio Analysis
🎧 To understand the audio data, waveforms and spectrograms were plotted for sample files, providing visual insights into the characteristics of different emotions.

## Feature Extraction 
Utilizing Python's LibROSA library, features were extracted from the audio files to facilitate model training. Key considerations included:

-  ⏱️ Uniform Duration: All audio clips were standardized to 3 seconds to ensure consistent feature extraction.
-  📈 Increased Sampling Rate: Doubling the sampling rate, while maintaining a constant sampling frequency, provided more detailed features, beneficial for smaller datasets.

The resulting feature arrays, each labeled with the corresponding emotion, served as input for model training.

## Model Development 
A Convolutional Neural Network (CNN) was employed, while alternative models, such as Multilayer Perceptrons (MLPs) and Long Short-Term Memory (LSTM) networks, were also tested but yielded lower accuracies.

## Conclusions
- __Model Performance:__ The model successfully detected five different male and female emotions from speech. The model distinguished between male and female voices with 100% accuracy and detected emotions with over 70% accuracy.
- __Live Testing Success:__ The model was tested on live recordings with emotions outside the training data and accurately identified the emotions, which suggests generalizability and potential real-world application.

## Future Improvements
- __Dataset Size:__ Future Work: The accuracy of emotion detection can be improved by increasing the size of the training dataset.
- __Additional Emotion Categories:__ Extend the range of emotions the model can detect to include more subtle emotions, such as frustration, excitement, or boredom, for more detailed emotional analysis.
- __Application Potential:__ This model could be applied to varoius contexts, such as mental health monitoring, integration into assistive technologies, and providing emotion-aware feedback in different settings. 
