# Labs Conversion Checklist
There are a few necessary steps in order to get a cadCAD model working with Labs in a way that allows it to be executed on our distributed execution environment:

- Create a `labs.py` file in the root of your project
- In your `labs.py` file, import the `exp` object from your model
- In your `labs.py` file, create a variable called `model_dir` and assign it the path to the directory that contains your model
- In your cadCAD configuration, supply a `model_id`

An example `labs.py`:
```python
from models.config import exp

model_dir = "models"
```

An example cadCAD configuration that specifies `model_id`:
```python
exp.append_configs(
    model_id="my-model",
    initial_state=genesis_states,
    partial_state_update_blocks=partial_state_update_blocks,
    update functions
    sim_configs=c
)
```