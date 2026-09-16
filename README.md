# Transforming-Machine
A machine that transforms meanings and texts.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Transform this idea into an essay, machine" \
  | uvx transforming-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install transforming-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
transforming-machine -a multilogue.txt
```
Or:
```bash
transforming-machine multilogue.txt > response.txt
```
Or:
```bash
transforming-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import transforming_machine
```
