# Simple RNN for IMDB Sentiment Analysis

This project demonstrates a basic implementation of a Recurrent Neural Network (RNN) for sentiment analysis using the IMDB dataset. The model is built with TensorFlow and Keras, and a Streamlit web application is used for deploying the model for real-time predictions.

---

## Requirements

Ensure you have the following installed:

- Python 3.x
- TensorFlow 2.x
- Keras
- Streamlit
- NumPy
- Pandas

---


## Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/simple-rnn-imdb.git
   cd simple-rnn-imdb


2 **Install dependencies: Using requirements.txt:**
pip install -r requirements.txt
Alternatively, manually install the libraries:
pip install tensorflow keras streamlit numpy pandas

**Project Structure**

## Project Structure

```plaintext
simple-rnn-imdb/
├── app.py              # Streamlit web application for deployment
├── model.py            # RNN model definition
├── utils.py            # Utility functions for data preprocessing
├── requirements.txt    # List of required libraries
└── README.md           # Project documentation


File Descriptions
app.py
Streamlit web application for deploying the RNN model. It allows users to input text (movie reviews) and receive a sentiment prediction (positive or negative).

model.py
Contains the RNN model implementation using Keras with TensorFlow. The model is trained on the IMDB dataset to predict whether a movie review is positive or negative.

utils.py
Includes utility functions for loading, tokenizing, padding, and preprocessing the IMDB dataset.

Steps
**1. Load the IMDB Dataset**
The IMDB dataset consists of 25,000 labeled movie reviews. Text data is preprocessed by:

Tokenizing: Splitting text into words or tokens.
Padding: Ensuring all sequences are of equal length.
Splitting: Dividing data into training and testing sets.
**2.Build the RNN Model**
The RNN model architecture includes:

Embedding Layer: Converts words into dense vectors.
LSTM Layer: Captures sequential dependencies in the data.
Dense Layer: Outputs a sigmoid-activated value to classify sentiment as positive or negative.
**3. Train the Model**
The model is trained using:

Loss Function: Binary Cross-Entropy
Optimizer: Adam
It learns to map text reviews to sentiment labels.
**4. Create the Streamlit App**
The Streamlit app allows users to:

Input a movie review.
Receive a real-time sentiment prediction.
**5. Run the Streamlit App**
Start the app locally by running:

streamlit run app.py

**6. Deploy the App**
You can deploy the application to platforms like:

Streamlit Community Cloud
Heroku
AWS, GCP, or Azure
Data Preprocessing
The IMDB dataset preprocessing pipeline includes:

Tokenization: Splitting text into individual tokens.
Padding: Ensuring uniform sequence length.
Text-to-Sequence Conversion: Converting text into numerical representations for model processing.
License
This project is licensed under the MIT License.


 **Nikhil Anil Warge**
