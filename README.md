# LangChain Multimodal Demo

This repository provides a Jupyter Notebook demonstrating how to build **multimodal pipelines** using [LangChain](https://github.com/langchain-ai/langchain).
The notebook integrates **text** and **image** inputs into a unified workflow, enabling tasks like visual reasoning, captioning, and multimodal question answering.

## 🚀 Features
- Integration of **LangChain** with multimodal inputs.
- Image and text processing with state-of-the-art models.
- Pipelines for:
  - Image captioning
  - Visual Q&A
  - Combining textual and visual reasoning
- Example prompts and chains for experimentation.

## 📂 Project Structure
```
.
├── langchain_multimodal_CLEAN.ipynb   # Cleaned: secrets removed, .env support
├── README.md                          # Project documentation
├── requirements.txt                   # Python dependencies
├── .env.example                       # Example env vars (no secrets)
└── .gitignore                         # Prevents committing secrets/artifacts
```

## 🛠️ Installation

```bash
pip install -r requirements.txt
```

## ▶️ Usage

1. **Create your local `.env`** (do not commit this file):
   ```bash
   cp .env.example .env
   # Then edit .env and put your real keys
   ```

2. **Run the notebook**:
   ```bash
   jupyter notebook langchain_multimodal_CLEAN.ipynb
   ```

3. The notebook loads your environment variables via `python-dotenv`. If you used a custom
   `LANGCHAIN_API_KEY` before, it will map it to `OPENAI_API_KEY` automatically.

## 🔐 Security Notes

- **Never** hardcode API keys in notebooks.
- Keep secrets in `.env` and ensure `.env` is listed in `.gitignore`.
- If you previously committed a secret, **revoke** it from the provider dashboard and generate a new one.

## 📜 License
MIT
