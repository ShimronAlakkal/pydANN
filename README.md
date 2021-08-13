# pydANN
        
#### is an open source, free-to-use, python package that you can use to make deep artificial neural network models. This package comes with a lot of customizations on the models that you create.


## Docs 

#### Inorder to make a model using pydANN, intanciate the class `ann()`
```python

model = ann()

```
#### Inorder to add hidden layers to the model, use the `add_hl( hidden_Layers_list , activations_for_each_layer + 1  )`

```python
# we are now going to add hidden layers to the model 

model.add_hl( [ 2,5,5 ] , activation_functions = ['relu', 'relu' ,'relu' ,'sigmoid'] )

# the above line adds to the model three hidden layers each of 2, 5 and 5 nodes, respectively. 
# The activation_functions should be 1 more in length so as to have one for each hl and for the output layer

```


algorithms under development for pydann:

    Artificial Neural Nets  
    Multi Layer Perceptrons
    K-means clustering
    K-nearest neighbours
    

[connect with me](https://www.instagram.com/shimron.alakkal)  
