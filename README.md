# Network For Emotion Recogntion from Facial Expressions using the FER dataset

This repository is a simple jupyter notebook that is trained on the Facial Expressions Recognition (FER2016) Dataset
Currently it does not include any additional data manipluation to avoid overfitting, but this might be added in the future

## Dataset
Simply load the FER2016 dataset from kaggle and place the csv in the ```data``` folder

## Requirements
- tensorflow >= 2.2
- jupyter notebook
- python >= 3.8
- numpy

the required virtual environment can be created from either the ```requirements.txt``` or the ```environment.yaml``` in the requirements folder

## workflow

run 
```bash
jupyter notebook
```

and go through all the codeblocks if you want to train the network from scratch.
the model also saves its architecture and weights to json and hdf file so they can be later on loaded for testing without re-training
to do so ; only run the blocks below the ```loading the model``` codeblock

## Accuracy

Our network achieves around 65% test accuracy
![accuracy](images/accuracy.png)

### loss

Here is the plot for the loss function
![loss function](images/loss.png)

it suffers from overfitting a lot so in future i might add data manipulation or experiment with the network layout
Feel free to contribute to the network layout for better accuracy.
