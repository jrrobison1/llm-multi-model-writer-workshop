# LLM Writer Workshop

[![CI](https://github.com/jrrobison1/llm-writer-workshop/actions/workflows/backend.yml/badge.svg)](https://github.com/jrrobison1/llm-writer-workshop/actions/workflows/backend.yml) [![CI](https://github.com/jrrobison1/llm-writer-workshop/actions/workflows/frontend.yml/badge.svg)](https://github.com/jrrobison1/llm-writer-workshop/actions/workflows/frontend.yml)

## Description

LLM Writer Workshop is a Python project that simulates a writing workshop with different roles: An writing agents, an editor, a fellow writer, and a publisher publishers. It uses various selectable AI models for different roles, including OpenAI's GPT-4 and GPT-3.5 Turbo; Anthropic's Claude Haiku, Sonnet, and Opus; Google's Gemini; and Mistral's small, medium, and large.

![Publisher Feedback](/.images/publisher_feedback.png "Publisher Feedback")


## Installation

### Backend
This project uses [Poetry](https://python-poetry.org/) for dependency management. To install the project dependencies, first install Poetry:
```sh
pip install poetry
```
Then run:
```sh
cd service
poetry install
```

#### API Keys
You will need API keys to run this project. Here are instructions for creating these api keys:<br />
OpenAI: https://help.openai.com/en/articles/4936850-where-do-i-find-my-openai-api-key<br />
Claude: https://docs.anthropic.com/claude/reference/getting-started-with-the-api<br />
Gemini: https://ai.google.dev/tutorials/get_started_web<br />
Mistral: https://docs.mistral.ai/

You can set up these api keys in a .env file. Copy the [``.env.example``](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FUsers%2Fjason%2FProjects%2Ftemp%2Fllm-multi-model-workshop%2F.env.example%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "/Users/jason/Projects/temp/llm-multi-model-workshop/.env.example") file to a new file named [``.env``](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FUsers%2Fjason%2FProjects%2Ftemp%2Fllm-multi-model-workshop%2F.env%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "/Users/jason/Projects/temp/llm-multi-model-workshop/.env") and replace the placeholders with your actual API keys:

```sh
cp .env.example .env
```

Alternatively, just create the following environment variables in your environment:<br />
```sh
export OPENAI_API_KEY=<your_openai_api_key>
export ANTHROPIC_API_KEY=<your_anthropic_api_key>
export GEMINI_API_KEY=<your_gemini_api_key>
export MISTRAL_API_KEY=<your_mistral_api_key>
```

<br /><br />

### UI
```sh
cd ui
npm install
```


## Usage
### Backend
```sh
cd service && poetry run python app.py
```

### Frontend
```sh
cd ui
npm start
```


## Testing
### Backend
This backend uses pytest for testing. To run the tests, use the following command:

```sh
cd service
poetry run pytest
```

### Frontend
```sh
cd ui
npm test
```

## License

This project is licensed under the terms of the MIT license.

## Contact

If you have any questions, feel free to reach out to me.
