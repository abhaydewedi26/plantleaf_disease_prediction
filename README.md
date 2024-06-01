# Plant Disease Classifier ( PlantPulse )

This project leverages a machine learning model to predict plant diseases from leaf images. The model is trained using a convolutional neural network (CNN) and can classify various plant diseases based on uploaded images.

## Features

- **Image Upload**: Users can upload images of plant leaves in JPG, JPEG, or PNG format.
- **Image Preprocessing**: The uploaded image is resized and normalized for model prediction.
- **Disease Prediction**: The pre-trained model predicts the disease class of the uploaded leaf image.
- **User Interface**: A simple and interactive UI built with Streamlit for ease of use.

## How It Works

1. **Model Loading**: The pre-trained model (accuracy - 97%) (`plant_disease_prediction_model.h5`) is loaded.
2. **Class Indices**: The class names are loaded from a JSON file (`class_indices.json`).
3. **Image Processing**: Uploaded images are resized to the target size (224x224), converted to numpy arrays, and normalized.
4. **Prediction**: The preprocessed image is fed into the model to predict the disease class, which is then displayed to the user.

## How to Use

1. **Upload an Image**: Click on the "Upload an image..." button and select an image of a plant leaf.
2. **Classify**: After the image is uploaded, click on the "Classify" button to predict the disease.
3. **View Prediction**: The predicted disease class will be displayed on the screen.

## Dependencies

- TensorFlow
- Pillow
- NumPy
- Streamlit

## Running the App

1. Clone the repository:
    ```bash
    git clone https://github.com/abhaydewedi26/PlantLeaf_Disease_Prediction.git
    ```
2. Navigate to the project directory:
    ```bash
    cd app
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Streamlit app:
    ```bash
    streamlit run main.py
    ```

