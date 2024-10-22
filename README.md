Team8 - Transformer Chatbot (Advanced Generative Chatbot Design and Implementation)
Overview
This repository contains the final project for Team 8 in AAI-520, focusing on building a generative-based chatbot using a Seq2Seq architecture with LSTM layers. The chatbot is trained on the Cornell Movie Dialogs Corpus to handle multi-turn conversations, adapt to context, and generate coherent responses.

Features
Multi-turn conversational chatbot based on movie dialogues.
Trained using Seq2Seq (Sequence-to-Sequence) architecture with LSTM encoder-decoder.
High accuracy and low loss during training.
Designed for scalability with future improvements planned for deployment via a web interface (Streamlit).
Project Structure
├── data/
│   ├── movie_lines.txt
│   ├── movie_conversations.txt
├── notebooks/
│   ├── Transformer_Chatbot.ipynb   # Jupyter notebook for model implementation and training
├── README.md                       # Project documentation
├── seq2seq_movie_chatbot.h5        # Saved model
├── requirements.txt                # List of required dependencies
Dataset
The dataset used for training the chatbot is the Cornell Movie Dialogs Corpus. It contains movie scripts, organized by lines and conversations, and is perfect for training a dialogue-based chatbot.

movie_lines.txt: Contains individual movie lines.
movie_conversations.txt: Contains conversation chains (multiple lines grouped into dialogues).

