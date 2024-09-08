
# 🤖 AI Chatbot with Enhanced Response Generation

Welcome to the **AI Post-Office Chatbot** project! This chatbot is designed to provide accurate and context-aware responses by leveraging a fine-tuned GPT-2 model and an intent-based approach. 

---
## 🚀 Features

- **Intent-Based Responses**: Uses predefined intents from `intents.json` to provide relevant answers to common queries.
- **Fuzzy Matching**: Employs fuzzy matching to handle slight variations in user inputs and improve response accuracy.
- **Fine-Tuned GPT-2 Model**: Integrates a GPT-2 model fine-tuned on your dataset to generate contextually relevant responses.
- **Fallback Mechanism**: Provides intelligent fallback responses when user inputs do not match any predefined intents.
- **Dynamic Response Generation**: Generates responses based on context to ensure more engaging interactions.

---
## 🛠️ Installation & Setup

1. **Clone the Repository**

   ```bash
   git clone https://github.com/jatinnama7/SIH_Chatbot_1752.git
   cd SIH_Chatbot_1752
   ```

2. **Install Dependencies**

   ```bash
   pip install torch transformers fuzzywuzzy

   ```

3. **Train the Model**

   Before running the chatbot, you need to train the model. Run the `trainer.py` script to fine-tune the GPT-2 model with your dataset.

   ```bash
   python trainer.py
   ```

4. **Run the Chatbot**

   Once the model is trained, start the chatbot with:

   ```bash
   python chatbot.py
   ```
   
## 📁 Files

- `intents.json`: Contains the intents, patterns, and responses used for the intent-based approach.
- `trainer.py`: Script to train the GPT-2 model using the dataset.
- `chatbot.py`: Main script to run the chatbot and handle user interactions.

## 🛠️ How It Works

1. **Training**: The `trainer.py` script fine-tunes the GPT-2 model using your dataset. This script prepares the model to generate relevant responses based on the training data.

2. **Chatbot**: The `chatbot.py` script loads the fine-tuned model and starts a conversation loop. It first tries to find a match for the user's input in the `intents.json`. If no match is found, it falls back to generating a response using the GPT-2 model.

3. **Intent Matching**: Uses fuzzy matching to identify the best matching intent and provides a relevant response based on predefined patterns and responses.

4. **Fallback Responses**: When no intent matches, the chatbot uses the GPT-2 model to generate a contextually appropriate response.

---
## 🔄 Future Improvements

- **Enhanced UI**: Consider developing a web-based interface for better user interaction.
- **Additional Features**: Integrate more sophisticated NLP techniques for improved conversation quality.
- **User Personalization**: Implement features to personalize responses based on user history and preferences.

## 📚 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Feel free to contribute to this project by opening issues or submitting pull requests. Your feedback and improvements are always welcome!

## 🌟 Acknowledgments

- **Transformers Library**: For providing the GPT-2 model and tokenizer.
- **FuzzyWuzzy Library**: For fuzzy matching capabilities.

---
