# AI Evals for Engineers and PM Course Reader Exercise

Jupyter notebooks for running and testing prompts from the [AI Evals for Engineers and PMs](https://github.com/ai-evals-course/) course reader exercises.

## Supported Providers

Use any of the following — pick whichever you have access to:

- **Hugging Face** — free, no credit card needed. Create a [free account](https://huggingface.co/join) and generate an [access token](https://huggingface.co/settings/tokens).
- **OpenAI** — paid. Requires an API key from [platform.openai.com](https://platform.openai.com/api-keys).
- **Anthropic** — paid. Requires an API key from [console.anthropic.com](https://console.anthropic.com/settings/keys).
- **Google Gemini** — free tier available. Requires an API key from [aistudio.google.com](https://aistudio.google.com/apikey).

You only need **one** provider to complete the exercises. If you don't want to spend money, Hugging Face or Google Gemini's free tier are great options.

## Getting Started

1. **Install uv** (if you don't have it yet):
  ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
  ```
2. **Initialize the project and install dependencies:**
  ```bash
   uv init
   uv add litellm python-dotenv ipykernel
  ```
   This creates a `pyproject.toml`, a virtual environment, and installs the required packages.
3. **Configure your API keys:**
  ```bash
   cp .env.example .env
  ```
   Edit `.env` and add the keys for the providers you want to use:
4. **Open and run `init.ipynb`** — select the `.venv` Python kernel, then run the cells for your chosen provider to verify everything works.
5. Once the test calls return a response, you're ready to start the exercises.

