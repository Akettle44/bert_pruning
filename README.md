# How to use `src/load_bert.py`?

Import the library:
```
from src.load_bert import load_all, load_config_and_tokenizer, load_model
```

Specify your model directory:
```
current_dir = os.getcwd() #This is assuming that your python notebook is in the notebooks/ directory
root_dir = os.path.dirname(current_dir) 
model_dir = os.path.join(root_dir, "models")
model_directory = os.path.join(model_dir, "any_model")
```

Specify the number of class labels and task type:
```
num_classes = 2
task_type = 'sequence_classification'
```

Load model, configuration, and tokenizer:
```
model, config, tokenizer = load_all(model_directory, num_classes, task_type)
```
    

