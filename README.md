# Datasaur-Case2_part2
This repo contains solution to the Datasaur hackathon task for text classification.

Solution ppt can be accessible via this [link](https://docs.google.com/presentation/d/17zr9uGyFILEj1IjM6vhpqpYaBHZxCFvn4CKDJOfGdSk/edit?usp=sharing)

Model can be run via this code snippet using mljar-supervised library:
```
import pickle
...

MODEL_PKL = 'automl_b.pkl'
...
automl = AutoML(...)
automl.fit(...)

#loading
with open(MODEL_PKL, 'rb') as f:
    model_json = pickle.load(f)
automl = AutoML()
automl.from_json(model_json)
```
