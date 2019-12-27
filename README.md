# GPT-2 simple on Chatistics data

This is a repository to fine-tune a GPT2 model on chat logs parsed with [Chatistics](https://github.com/MasterScrat/Chatistics).

# Install
```
pip install -r requirements.txt
```

# Usage

1. Parse chat logs with [Chatistics](https://github.com/MasterScrat/Chatistics)
2. Move generated pickle files to the folder `chatistics_data`
3. Fine tune a GPT2 model
```
python finetune.py --run-name run1
```
You can stop any time (use Ctrl-C) and continue (if you use the same `run-name`). Fine the model until you see the desired output. The model should generate output of the form:
```
bot: hello
you: hi there!
bot: how are you?
...
``` 
4. Interact with the finetuned model and speak to yourself!
```
python interact.py --run-name run1
```
