<<<<<<< HEAD
# Local_LLM_Inference
=======
```markdown
# Local LLM Inference

Run prompts from a CSV file through a local Ollama model and save the generated responses to a CSV file.

## Prerequisites

- Python 3
- [Ollama](https://ollama.com/) installed and running
- The `llama3.2` model available locally:

	```bash
	ollama pull llama3.2
	```

- Install the Python dependencies:

	```bash
	pip install pandas ollama
	```

## Input data

Create `dataset/prompts.csv` with the columns `prompt_id`, `domain`, and `prompt`. For example:

```csv
prompt_id,domain,prompt
1,general,Explain what a local language model is.
```

## Run

Save the provided Python script in the project directory and run it with Ollama active:

```bash
python your_script.py
```

The script processes each row in `dataset/prompts.csv` and writes the prompt ID, domain, prompt, and model response to `dataset/llm_responses.csv`. The output file is overwritten on each run.
```
>>>>>>> dcbf83c (Added README file)
