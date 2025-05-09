Emotion Detection Using BERT (Final Year Project)

This project is designed to detect human emotions from short texts like tweets or comments. It uses a deep learning model called *BERT (Bidirectional Encoder Representations from Transformers)* and is trained on the *GoEmotions dataset* which contains 28 emotion labels.

The goal is to classify a sentence into one of these emotions with high accuracy, and visualize the prediction using simple charts.


##  About the Project

This is a final year university project that applies advanced NLP (Natural Language Processing) techniques for emotion detection. The system uses a pre-trained *BERT model* which is fine-tuned on the *GoEmotions dataset* from Google.

### Emotion labels include:
joy, anger, sadness, love, excitement, fear, surprise, gratitude, curiosity, and more (total 28 classes including neutral).

The project covers:
- Data loading and preprocessing
- Fine-tuning the BERT model
- Evaluating the model
- Predicting emotion for new text
- Generating bar and pie charts for output


##  Project Structure

emotion-detection/
│
├── train_model.py # Model training script
├── emotion_predictor.py # Predicts emotion from text
├── evaluate_model.py # Evaluates model performance
├── visualize.py # Generates bar and pie charts
├── notebook.ipynb # Full project steps in Colab
├── requirements.txt # List of libraries needed
└── README.md # Project overview



##  Sample Output

*Input*:
"Loving the new AI art tool!"

*Output*:
Predicted Emotion: love (69.3%)



A chart is also generated showing the top 5 emotions with their confidence scores.


##  How to Run

### 1. Clone the Repository

git clone https://github.com/your-username/emotion-detection.git
cd emotion-detection
2. Install Required Libraries
pip install -r requirements.txt
3. Run Prediction Code

from emotion_predictor import predict_emotion

text = "I'm excited about the new semester!"
emotion, confidence = predict_emotion(text)
print(f"Emotion: {emotion} ({confidence * 100:.1f}%)")
 Model Training Summary
Model Used: BERT-base (uncased)
