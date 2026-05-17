# Silent-Machine
Silent machine.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Think, but stay silent, machine." \
  | uvx silent-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install silent-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
silent-machine -a multilogue.txt
```
Or:
```bash
silent-machine multilogue.txt > response.txt
```
Or:
```bash
silent-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import silent_machine
```
