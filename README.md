# Material_Classifier_TeachableMachine

This repository presents an image recognition model developed using Google's Teachable Machine, specifically designed to classify various materials into one of three fundamental categories: **Conductors, Insulators, or Semiconductors**. This project demonstrates the process of training a custom image classification model and integrating it into a Python application for practical use.

---

## Project Overview

This project addresses the task of visually identifying material types based on their appearance, a common challenge in various scientific and engineering fields. The workflow involves leveraging a user-friendly platform (Teachable Machine) for model training, followed by creating a Python script to deploy and utilize the trained model for predictions.

---

1.  **Model Training:** An image recognition model was trained using Google's Teachable Machine.
    * **Classes:** The model was meticulously trained to classify images into the following three distinct material types:
        * `Conductor` (e.g., metals like copper, aluminum)
        * `Insulator` (e.g., plastic, rubber, wood)
        * `Semiconductor` (e.g., silicon wafers, microchips)
    * **Model Evaluation:** <img width="2830" height="1516" alt="trained model result" src="https://github.com/user-attachments/assets/e4035faa-569e-4eb9-966b-b993e0369625" />
The model was thoroughly evaluated within Teachable Machine's environment. It achieved high accuracy (over 95%) on the validation data, demonstrating a strong ability to accurately distinguish between the visual characteristics of conductors, insulators, and semiconductors.

2.  **Model Export:** The trained model was downloaded in TensorFlow/Keras format.
    * The necessary files, `keras_model.h5` (containing the model's architecture and learned weights) and `labels.txt` (listing the names of the trained classes), are included in this repository.

3.  **Prediction Script:** A Python script was written to load this model, accept an input image, and predict its class.
    * The script, named `predict_material.py`, serves as the interface for the trained model.
    * It intelligently loads the pre-trained Keras model and the associated class labels.
    * It incorporates essential image preprocessing steps (such as resizing to 224x224 pixels and normalization of pixel values) to prepare any input image for correct interpretation by the model.
    * Upon processing, it performs a prediction and clearly outputs the classified material type along with a confidence score, indicating the model's certainty.

---

## Repository Contents:

* `predict_material.py`: The Python script designed to load the material classification model and perform predictions on new images.
* `keras_model.h5`: The core pre-trained neural network model, exported in HDF5 format from Google Teachable Machine.
* `labels.txt`: A simple text file listing the names of the three material classes (`Conductor`, `Insulator`, `Semiconductor`) in the order the model expects.
* `gold.jpg`: An illustrative example image of a material. This image is used to demonstrate the functionality of the `predict_material.py` script.
* `material_classifier_output.png`: A screenshot showcasing the successful output of the `predict_material.py` script, displaying a classification prediction and confidence score.
* `README.md`: This comprehensive document, providing an overview of the project, detailed task descriptions, and instructions for use.

---

[اسمك هنا / Your GitHub Username]
