# pydANN
        
#### is an open source, free-to-use, python package that you can use to make deep artificial neural network models. This package comes with a lot of customizations on the models that you create.


## Docs 

#### Inorder to make an Artificial Neural Network model using pydANN, intanciate the class `ann()`
```python

model = ann()

```
#### Inorder to add hidden layers to the model use the method `add_hl( hidden_Layers_list , activations_for_each_layer + 1  )`

```python
# we are now going to add hidden layers to the model 

model.add_hl( [ 2,5,5 ] , activation_functions = ['relu', 'relu' ,'relu' ,'sigmoid'] )

# the above line adds to the model three hidden layers each of 2, 5 and 5 nodes, respectively. 
# The activation_functions should be 1 more in length so as to have one for each hl and an activation for the output layer

```

#### To train the model, use the `fit( xtrain, ytrain, epoch = 50, learning_rate = 0.01, verbose = 0,decay = True, decay_iter = 5, decay_rate = 0.9, stop_decay_counter = 100, loss_function = 'mse'  )` method

```python
# you can also register the training data before you train the model.

model.fit( train_x , y_train )  # this is the basic implementation of the method without any alteration
```

**epoch :  The number of iterations to train the model**

**learning_rate : The value with which the algorithm optimizes weights and biases**

**verbose : When put 0, verbose is False ( There won't be data printing ) if set to another value other than 0, then the data is printed after each verbose interval**

**decay : This value optimizes the learning_rate when set to True**

**loss_function : The function using which the loss is calculated. Loss function option : 'mse' , 'rmse'**

**decay_rate : The fractional value with which the learning rate is altered**



#### To plot the change in the cost(s) after each epoch, use `plot_cost_to_epoch()`
```python
model.plot_cost_to_epoch()
```

#### To plot the change in learning_rate after each epoch, use `plot_lrc_to_epoch()`
```python
model.plot_lrc_to_epoch()
```
    
#### To predict on test data, use the function `predict( xtest )`
```python
y_predictions = model.predict( xtest )
```

#### To evaluate the model base on Mean Squared Error, use `mse_model_eval( ytest,ypreds )`
```python
model.mse_model_eval( ytest,ypreds )
```

#### To save the current trained model use method `save_model( file = 'pydann_model.dat' )`
```python

# 'file' is the name of the file in which the model would be saved and it has to be a .dat file
model.save_model()     # to save the model as pydann_model.dat just call the function like this

# to customize the name of the file in which the model should be saved , change 'file'
model.save_model( file = 'model.dat' )
```

#### To use the saved model use method `use_model( path )`
```python
# path is the file path ( directory ) to the saved model
model.use_model( )
```

#### To dispose the model and clear memory use the `dispose_model()` method
```python
model.dispose_model()
```

#### To get the documentations locally on your device about the class use 
```python
model.help()
```                             

#
[connect with me](https://www.instagram.com/shimron.alakkal)  
