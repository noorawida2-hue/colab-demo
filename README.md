# colab-demo

A beginner-friendly collection of Google Colab notebooks.

## Creative ideas

[`creative_ideas.ipynb`](creative_ideas.ipynb) asks for an everyday object and uses the OpenAI Responses API with model `gpt-6-luna` to suggest **one unusual, practical use**.

### Run in Google Colab

1. Open [Google Colab](https://colab.research.google.com/), choose **File > Upload notebook**, and select `creative_ideas.ipynb` from this folder.
2. Run the first code cell to install or update the OpenAI Python SDK in the Colab runtime.
3. Run the next code cell and enter an everyday object, such as a mug.
4. Enter your OpenAI API key in the hidden `getpass` prompt. The notebook prints the generated idea.

You need an [OpenAI API key](https://platform.openai.com/api-keys), API credit, and access to `gpt-6-luna`. API requests may incur charges. If the request fails, check your key, API credit, model access, and internet connection, then rerun the cell.

### Keep your key private

Enter your key only in the runtime prompt. Never paste it into source code, print it, put it in a file, or commit it to Git. The notebook uses the key in memory and contains no saved outputs or credentials. Disconnect and delete the Colab runtime when you finish. Clear outputs and check cells before sharing or committing a notebook.

The example follows the [official OpenAI Python SDK documentation](https://developers.openai.com/api/reference/python), using `client.responses.create(...)` and `response.output_text`.

## Hello Colab

[`hello_colab.ipynb`](hello_colab.ipynb) demonstrates Python addition and multiplication without extra packages.
