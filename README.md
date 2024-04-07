# MiniGPT

This is a course project on Machine Learning, a Bayesian Perspective in TU Delft EE Signal & Systems.
The code is heavily referred from https://github.com/karpathy, and some code pieces are permitted by the author to be used in public.

** Dataset: English text: "Tiny_Shakespeare" around 1M characters. 
          and "goods_zh" contains 13M comments on online shopping products.

The fine-tuning file contains the code used to fine-tune the pre-trained model.

Generated texts and images contain everything used in the project.

MiniGPT + Bigram file contains the code and description for both models.

The tokenizer file contains regex and a basic tokenizer pre-defined to use.


# Project Description:

Project 6: Build Your Mini-GPT

The advent of transformer models like GPT has revolutionized Machine Learning (ML) and Deep Learning (DL). Building a mini-GPT model offers invaluable practical experience with core concepts such as attention mechanisms, language modeling, and neural network fine-tuning. This project not only solidifies a theoretical understanding but also equips students with hands-on skills that are essential in the rapidly evolving field of AI.

Steps to Build the Mini-GPT Model

Set up your Python environment and install necessary libraries like PyTorch.
Dive into the GPT architecture, focusing on its transformer mechanisms.
Implement the mini-GPT architecture with a transformer block in PyTorch.
Process your dataset for training, including tokenization and formatting.
Train your model, tuning hyperparameters for optimal performance.
Validate the model’s performance on a separate dataset.
Fine-tune the model on a chosen downstream task (optional)
Test the model to evaluate its performance on unseen data.
Document the process, architecture, and performance metrics.

# Instructions to run the code
To run the code, you need to make sure 'cuda' can be used on your computer since the LLM needs a GPU to train.

**What we did:**
Implemented Bigram and MiniGPT models compared to English and Chinese text.
Bigram model produced poor text, while MiniGPT generated nonsensical text.
Introduced BasicTokenizer and RegexTokenizer, with RegexTokenizer significantly improving text quality.
Addressed underfitting and overfitting to enhance model generalization.
Fine-tuned pre-trained GPT-2 model on English text, yielding satisfactory results.

**Future development:**
Future development focuses on adding a cross-attention mechanism for diverse text tasks and conducting hyper-parameter searches.
Investigating effective methods for evaluating text quality in future endeavors.

**Model Performance: Bigram vs. MiniGPT**
Bigram model: Decreasing losses, but incoherent text due to token-level approach.
MiniGPT model: Achieved maximum generalization with improved coherence, thanks to the attention mechanism.
Chinese text is slightly better than English, but challenges remain with the character-level approach.


**Tokenizer Effect**
Tokenizer introduced for better MiniGPT-generated text.
Training time and token length varied by tokenizer.
Larger dictionaries boosted accuracy but extended training.
RegexTokenizer improved text quality over BasicTokenizer.
2048-vocabulary RegexTokenizer yielded concise tokens, enhancing text quality.


