# Modes-of-Thought
Modes of thought.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: How should we think about it, machine?" \
  | uvx modes-of-thought \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
pip install modes-of-thought
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
modes-of-thought multilogue.txt
```
Or:
```bash
modes-of-thought multilogue.txt > output.txt
```
Or:
```bash
modes-of-thought multilogue.txt > tmp && mv tmp multilogue.txt
```
Or:
```bash
cat multilogue.txt new_turn.txt | modes-of-thought
```
Or:
```bash
cat multilogue.txt new_turn.txt | modes-of-thought > tmp && mv tmp multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: What do you think, Modes-of-Thought?") \
  | modes-of-thought
```
Or:
```bash
cat multilogue.txt new_turn.txt | modes-of-thought > tmp && mv tmp multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | modes-of-thought \
  | summarizing-machine | judging-machine > summary_judgment.md
```

Or use it in your Python code:
```Python
# Python
import modes_of_thought
```
