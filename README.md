# Plant Disease Recognition using CNN

This project aims to develop a Convolutional Neural Network (CNN) model for recognizing plant diseases. The CNN model is trained to classify images of plant leaves into different disease categories. The project includes building the CNN model in a Google Colab notebook, importing it to a local machine, deploying it using a Streamlit web application, and further deploying it as a Docker container.

## Project Structure

- **Colab Notebooks**: Contains the Jupyter notebooks used for building and training the CNN model on Google Colab.
- **Trained Models**: Stores the trained CNN model(s) exported from the Colab notebooks.
- **App**: Contains the source code for the Streamlit web application (`main.py`) used to deploy the model.
- **Docker**: Holds the Dockerfile used to build the Docker image for deploying the application as a container.
- **Datasets**: Contains datasets used for training and testing the CNN model.
- **Documentation**: Stores any additional documentation related to the project.

## Setup Instructions

1. **Building the CNN Model (Google Colab)**
   - Open the Jupyter notebooks in the `Colab Notebooks` directory using Google Colab.
   - Follow the instructions in the notebooks to build and train the CNN model using the provided datasets.
   - Export the trained model(s) to the `Trained Models` directory.

2. **Local Setup**
   - Clone this repository to your local machine.
   - Install the necessary dependencies specified in `requirements.txt` using pip:
     ```
     pip install -r requirements.txt
     ```

3. **Deploying the Streamlit App**
   - Navigate to the `App` directory.
   - Run the Streamlit app using the following command:
     ```
     streamlit run main.py
     ```

4. **Docker Setup and Deployment**
   - Ensure Docker is installed on your local machine.
   - Navigate to the `Docker` directory.
   - Build the Docker image using the provided Dockerfile:
     ```
     docker build -t plant-disease-recognition .
     ```
   - Run the Docker container:
     ```
     docker run -p 8501:8501 plant-disease-recognition
     ```
