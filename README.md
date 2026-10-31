# colab-demo

A beginner-friendly collection of Google Colab notebooks.

## Creative ideas

[`creative_ideas.ipynb`](creative_ideas.ipynb) asks for an everyday object and uses the OpenAI Responses API with model `gpt-6-luna` to suggest **three unusual, practical uses**, displayed as a numbered list (1, 2, 3).

### Run in Google Colab

1. Open [Google Colab](https://colab.research.google.com/), choose **File > Upload notebook**, and select `creative_ideas.ipynb` from this folder.
2. Run the first code cell to install or update the OpenAI Python SDK in the Colab runtime.
3. Run the next code cell and enter your OpenAI API key once in the hidden `getpass` prompt.
4. Enter an everyday object, such as an umbrella. The notebook prints three numbered ideas.
5. Enter another object at the next prompt to keep going without restarting the notebook.
6. Type `exit` (any capitalization) to finish. To use a different API key, exit and rerun the cell.

You need an [OpenAI API key](https://platform.openai.com/api-keys), API credit, and access to `gpt-6-luna`. API requests may incur charges. If the request fails, check your key, API credit, model access, and internet connection, then try the object again. Blank input is rejected without making an API request. If the response does not contain three valid ideas, the notebook asks you to try again instead of displaying an incomplete list. Errors are shown as friendly messages without raw exception details or the API key.

### Keep your key private

Enter your key only in the runtime prompt. Never paste it into source code, print it, put it in a file, or commit it to Git. The notebook uses the key in memory and contains no saved outputs or credentials. Disconnect and delete the Colab runtime when you finish. Clear outputs and check cells before sharing or committing a notebook.

The example follows the [official OpenAI Python SDK documentation](https://developers.openai.com/api/reference/python), using `client.responses.create(...)` and `response.output_text`.

## Hello Colab

[`hello_colab.ipynb`](hello_colab.ipynb) demonstrates Python addition and multiplication without extra packages.
