# Programming-Machine
A Machine that writes programs.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Write a program doing that, machine." \
  | uvx programming-machine \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
pip install programming-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
programming-machine multilogue.txt
```
Or:
```bash
programming-machine multilogue.txt new_turn.txt
```
Or:
```bash
cat multilogue.txt | programming-machine
```
Or:
```bash
cat multilogue.txt | programming-machine > tmp && mv tmp multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: What do you think, Programming-Machine?") \
  | programming-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | programming-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | programming-machine >  tmp && mv tmp multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | programming-machine \
  | summarizing-machine | judging-machine > summary_judgment.md
```

Or use it in your Python code:
```Python
# Python
import programming_machine
```
