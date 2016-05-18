In this LeNet model, you could easily train your LeNet model and then visualize the features learned by
this model. To visualize them, I change the inputs into tf.Variables and look for what kind of inputs could 
result in perticular neuron to reach its maximium activation (like Google's Deepdream). Of course, at this 
time all weights are not trainable except the inputs. To converge, I use L2 norm of regularization (on the 
inputs).

Working flow:
1. load data
2. train a LeNet model
3. record the model's weights
4. build a LeNet model with 'trainable = False' and train it
5. plot the features

See more details in the source codes, working flow is coded outside the LeNet class in the codes.
