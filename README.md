## Movie Glossary Bot - README

### Project Overview

This repository contains three versions of a **Movie Glossary Bot** designed to engage users in conversations, focusing on movie-related topics. The chatbot was developed as part of the **University of San Diego’s Natural Language Processing and GenAI (AAI-520)** course, with contributions from **Yash Chaturvedi, Narendra Fadnavis, and Joseph Friedel**. 

The three versions of the bot use different models and training datasets, and this README will outline the details of each version, including links to the implementation and instructions on how to run the models.

### Dataset

The dataset used in this project consists of **movie-related conversations**, which were used to train the models in different capacities:
- **100 Conversations**: A small subset for initial training and testing.
- **All Conversations**: The complete dataset for more extensive training.
- **3,000 Conversations**: A large training set to improve model generalization.

The dataset is structured as conversation pairs, where each input (user query) is matched with an appropriate response (bot response). This setup allows the models to learn dialogue generation.

---

### Versions of the Bot

#### 1. **Model 1: GPT-2 (100 Conversations)**
- **Description**: This is the first version of the Movie Glossary Bot. It uses a **GPT-2** based model trained on a small dataset of 100 movie-related conversations. The smaller dataset allows for quicker training, but with limited context understanding and response generation capability.
- **Model Architecture**: GPT-2
- **Training Data**: 100 conversations
- **Training Time**: Short

---

#### 2. **Model 2: Seq2Seq (All Conversations)**
- **Description**: This version utilizes a **Seq2Seq model** (Encoder-Decoder architecture) trained on the entire dataset of movie conversations. With all available data, this version is capable of more complex and varied conversations. Seq2Seq architecture is well-suited for natural language understanding and response generation across multiple turns.
- **Model Architecture**: Seq2Seq (LSTM-based Encoder-Decoder)
- **Training Data**: All conversations from the dataset
- **Training Time**: Longer compared to Version 1 due to the larger dataset

---

#### 3. **Model 3: GPT-2 (3,000 Conversations)**
- **Description**: The third version revisits the **GPT-2 model** but is trained on a much larger dataset, containing **3,000 conversations**. This version provides a balance between performance and complexity, offering better conversational abilities than the first version with a quicker response time than the Seq2Seq model. A web interface is provided to make it easy for users to interact with the bot.
- **Model Architecture**: GPT-2
- **Training Data**: 3,000 conversations
- **Training Time**: Moderate
- **Web Interface**: Small web interface included for easy interaction.

---

### Dataset Details

The dataset used to train the models consists of movie-related conversations in a question-response format. Each entry in the dataset represents a pair of conversational turns, with the first part being the user’s question or statement and the second part being the appropriate bot response. The dataset was divided into multiple subsets for training different versions of the model:
- **100 Conversations**: Used in Model 1 (small training set).
- **All Conversations**: Used in Model 2 (comprehensive dataset).
- **3,000 Conversations**: Used in Model 3 (larger training set).

---

### Dependencies

Ensure you have the following dependencies installed before running any of the models:
- Python 3.x
- PyTorch
- TensorFlow (for Seq2Seq model)
- Transformers (Huggingface for GPT-2 models)
- Flask (for the web interface in Model 3)


### Future Work

- **Fine-Tuning**: Additional fine-tuning can be performed on the models to improve performance with more diverse conversations.
- **Generalization**: Test the model on unseen datasets to assess generalization capability.
- **Deployment**: Expand the web interface and deploy the chatbot as a cloud-based service.

---

### Contributors
- **Yash Chaturvedi**
- **Narendra Fadnavis**
- **Joseph Friedel**
