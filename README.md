# Tensorflow-pruning
## Tensorflow implementation of the two pruning techniques :
1- Weight pruning which focuses on individual weights and set them to zero if they are less than a certain threshold value. 

2- Neuron pruning which set whole columns to zero according to their L2 Norm values

## Guide
Just run the notebook in colab and every thing will run smoothly.

## Ambiguities
In this piece of code , the step is "2" because odd values in the array of trainable_weights stands for the biases
```
for i in range(0,len(model.trainable_weights),2):
    Weights.append(model.trainable_weights[i].numpy().reshape(-1))
```
