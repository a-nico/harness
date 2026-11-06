# harness

Learn to build an agent, starting with `1_calling_model.ipynb`.

Set up a local Python environment from this directory:

```bash
uv venv --seed .venv
uv pip install --python .venv/bin/python ipykernel openai python-dotenv
```

In VS Code, open the notebook and choose **Select Kernel → Python Environments → .venv**
(`/home/anon/harness/.venv/bin/python`). Then run one cell at a time.

Fill in `.env` with your Azure API key and full v1 base URL.
Set the model deployment name directly in the notebook's `model` argument.
`.env` is ignored by Git.

The virtual environment keeps notebook packages separate from the system Python.
`--seed` includes pip so the notebook's `%pip` cell also works.

Setup reference: [uv with Jupyter and VS Code](https://docs.astral.sh/uv/guides/integration/jupyter/).
