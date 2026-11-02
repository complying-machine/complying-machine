# Complying-Machine
A machine that complies with rules and orders.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Comply with this set of rules, machine." \
  | uvx complying-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install complying-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
complying-machine -a multilogue.txt
```
Or:
```bash
complying-machine multilogue.txt > response.txt
```
Or:
```bash
complying-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import complying_machine
```
