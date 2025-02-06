# Tutorial: Connect to Gemini Using Python

This tutorial will guide you through the steps to connect to Gemini using Python. We will use Google's Gemini API to interact with the model.

## Prerequisites

Before proceeding, ensure you have the following:
- Python installed (3.7+ recommended)
- An API key from Google for Gemini access
- `google-generativeai` Python package installed

## Installation

Install the required package using pip:

```sh
pip install -q -U google-genai
```

## Connecting to Gemini

Here's a basic Python script to connect to Gemini and generate a response:

```python
from google import genai


client = genai.Client(api_key='your_api_key_here')

response = client.models.generate_content(
    model="gemini-2.0-flash",
    contents="Explain how AI works in less than 100 words",
)

print(response.text)
```

## Notes
- **Replace `your_api_key_here` with your actual API key** to authenticate the request.
- If you encounter any issues, ensure that your API key is valid and has the necessary permissions.

## Next Steps
- Explore the Gemini API documentation for advanced usage.
- Experiment with different prompts and parameters to fine-tune responses.

Happy coding! 🚀

