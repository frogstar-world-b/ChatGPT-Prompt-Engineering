# ChatGPT-Prompt-Engineering

The notebooks are inspired by a [DeepLearning.AI course](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/) on the topic of prompt engineering. They cover best practices for prompt engineering and demonstrate how to use LLM APIs for a range of tasks, including:

- Summarization (e.g., condensing user reviews for conciseness)
- Inference (e.g., sentiment analysis, topic extraction)
- Text transformation (e.g., translation, spelling and grammar correction)
- Text expansion (e.g., automated email composition)
- Building a custom chatbot

## Requirements

To set up the project and use the notebooks, follow these requirements:


1. Make sure you have Python installed on your system (Python >= 3.6).

2. Install the required Python packages using pip:

   ```bash
   pip install openai python-dotenv
   ```

3. Create a `.env` file in the project directory.

4. Add your OpenAI API key to the `.env` file as follows:

   ```
   OPENAI_API_KEY="your_openai_api_key_here"
   ```

   Replace `"your_openai_api_key_here"` with your actual OpenAI API key.

5. Save the `.env` file.

6. In your Python script, import the necessary libraries and configure the OpenAI API client using the `dotenv` package:

   ```python
   import openai
   import os
   from dotenv import load_dotenv, find_dotenv

   # Load environment variables from .env file
   load_dotenv(find_dotenv())

   # Configure the OpenAI API client with your API key
   openai.api_key = os.getenv("OPENAI_API_KEY")
   ```

