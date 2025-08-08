# Arabic-To-SQL
This project focuses on translating Arabic natural language questions into SQL queries using a fine-tuned multilingual mBART50 model.
It leverages the Hugging Face Transformers library, a custom Arabic-to-SQL dataset, and robust preprocessing techniques to enable accurate SQL generation from Arabic prompts.
The system is ideal for Arabic-speaking users who want to interact with databases without needing to know SQL syntax.

Key Features:
  - Dataset preprocessing: Normalizes Arabic text (diacritics, characters), tokenizes SQL queries, and prepares the data from .jsonl files.
  - Model training:
    Uses facebook/mbart-large-50 pretrained model.
    Fine-tunes it on Arabic-to-SQL pairs using Hugging Face Trainer.
  - Testing and inference:
    Accepts user-input Arabic questions.
    Outputs the corresponding SQL queries.
  - Tools used:
    transformers, datasets, pandas, torch
    MBart50Tokenizer for multilingual tokenization (Arabic to SQL/English)
  - Training configuration:
    Trained for 3 epochs using PyTorch + Hugging Face Trainer.
    Model saved and archived to Google Drive for reuse.
