# Next Word Prediction Using GRU RNN

## Project Overview
This project focuses on developing a deep learning model for predicting the next word in a sequence using Gated Recurrent Unit (GRU) networks. GRUs are highly efficient for sequence-based tasks, offering similar performance to LSTMs but with fewer parameters. The dataset used is Shakespeare's *Hamlet*, providing a rich and challenging source of text for training and evaluation.

---

## Steps and Methodology

1. **Data Collection**  
   The text of *Hamlet* by William Shakespeare is used as the dataset, sourced from the NLTK library. This complex text serves as an excellent testbed for natural language processing.

2. **Data Preprocessing**  
   - The text is tokenized into words and transformed into sequences.
   - Sequences are padded to ensure uniform input length.
   - The data is split into training and testing sets for model development and evaluation.

3. **Model Development**  
   - The model architecture includes:
     - **Embedding Layer**: To learn word representations.
     - **Two GRU Layers**: To capture temporal dependencies in word sequences efficiently.
     - **Dropout Layers**: To prevent overfitting.
     - **Dense Layer with Softmax Activation**: To predict the next word's probability distribution across the vocabulary.

4. **Model Training**  
   - The model is trained on the preprocessed data.
   - **Early Stopping** is employed to monitor validation loss and prevent overfitting.

5. **Model Evaluation**  
   The trained model is tested on example sentences to assess its accuracy in predicting the next word. The results demonstrate the model's capability to handle Shakespearean language.

6. **Deployment**  
   A **Streamlit** web application is developed for real-time usage. Users can input a sequence of words, and the application predicts the next word based on the trained GRU model.

---

## Features
- **Dataset**: Shakespeare's *Hamlet* from NLTK.
- **Model**: GRU-based architecture designed for sequence prediction.
- **Training Enhancements**: Includes early stopping to optimize training performance.
- **User Interaction**: Real-time next-word prediction via a web application.

---

## How to Use
1. Clone the repository.
2. Install the required dependencies (`requirements.txt`).
3. Train the model or load the pre-trained model.
4. Run the Streamlit app to test the next-word prediction feature.

---

## Future Enhancements
- Expand the dataset to include more works from Shakespeare or other authors.
- Incorporate more advanced NLP techniques such as transformers.
- Improve the web application by adding visualization of predictions or model performance.

---

## Conclusion
This project demonstrates how GRU networks can effectively predict the next word in a text sequence, even when trained on complex datasets like *Hamlet*. The deployment via Streamlit makes the model accessible and user-friendly for real-time interaction.

---