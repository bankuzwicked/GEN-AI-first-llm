# 🎬 Movie Plot Generator

An AI-powered movie plot generator that creates unique storylines from your prompts using fine-tuned distilgpt2.



![image](https://github.com/user-attachments/assets/41f41282-3f65-41f6-a90d-48a1df1d1a34)


![image](https://github.com/user-attachments/assets/5a5321cb-c572-4b59-88a4-ad7619865dfa)




## ✨ Features

- Generate creative movie plots from simple prompts
- Fine-tuned on Wikipedia movie plot summaries
- User-friendly Streamlit web interface
- Text generation with customizable parameters
- Lightweight implementation using distilgpt2

## 📋 Overview

This project showcases how transformer-based language models can be fine-tuned for creative text generation. By training Hugging Face's `distilgpt2` on movie plot summaries, the model learns the structure and patterns of storytelling in cinema, allowing it to generate unique and sometimes surprising plot ideas from minimal input.

The entire system is wrapped in a Streamlit application, making it accessible to users without technical knowledge.

## 🛠️ Technologies Used

- **Model**: distilgpt2 (GPT2LMHeadModel)
- **NLP Libraries**: Hugging Face `transformers`, `datasets`
- **Backend**: PyTorch
- **Data Handling**: Pandas
- **Web Interface**: Streamlit
- **Supporting Tools**: scikit-learn, tqdm, matplotlib, tokenizers

## 📚 Dataset

The model was trained on a subset of the [Wikipedia Movie Plots Dataset](https://www.kaggle.com/datasets) from Kaggle, consisting of 1,000 plot summaries. This focused training approach allowed for efficient fine-tuning while maintaining narrative coherence.

## 💻 Usage

1. Enter a prompt in the text field (e.g., "A thriller about a detective who")
2. Adjust generation parameters if desired:
   - **Temperature**: Higher values (e.g., 0.9) create more diverse outputs
   - **Max Length**: The maximum number of tokens to generate
   - **Top-k/Top-p**: Sampling parameters for text generation
3. Click "Generate Plot" and watch as the AI creates a unique movie storyline!

## 📊 Training Process

The model was trained for 10 epochs with a learning rate of 2e-5, achieving a final loss of approximately 3.61. Training utilized an 80/20 train/test split over 2,740 global steps.

## 🔮 Future Enhancements

- Training on the complete dataset (34,000+ plots)
- Adding genre conditioning to generate plots in specific styles
- Upgrading to larger models for more coherent generation
- Implementing user feedback collection for reinforcement learning
- Cloud deployment on Hugging Face Spaces or similar platforms

## 📝 Example Outputs

**Prompt**: "A short film about a pilot who"  
**Generated**: "is trapped in an underground submarine. The Girl At Home (1970) tells the story of a young woman who discovers her husband has been kidnapped by a mysterious organization. As she investigates, she uncovers a conspiracy involving government experimentation..."

## 👏 Acknowledgments

- [Hugging Face](https://huggingface.co/) for their incredible transformers library
- [Streamlit](https://streamlit.io/) for making web app development straightforward
- [Kaggle](https://www.kaggle.com/) for hosting the Wikipedia Movie Plots dataset

## 📩 Contact

For questions or suggestions, feel free to open an issue or connect on [LinkedIn](https://www.linkedin.com/in/subham-das-3b2624147).
