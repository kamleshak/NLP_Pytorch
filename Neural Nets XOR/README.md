
# Neural Net for XOR with Pytorch

It shows XOR implementation in pytorch along with few key definations in artificial neural nets.






## Definations in Neural Nets:
### What is a neural network neuron?
Neural Network Neuron: Neurons in neural network are similar to that of biological neurons. Picture below depicts the difference between biological neuron and artificial neuron.

 ![alt text](https://github.com/kamleshak/NLP_Pytorch/blob/main/Neural%20Nets%20XOR/neuron.png?raw=true)

A neuron takes input, processes it and gives output. Mathematically artificial neuron takes the inputs and multiplies them by their weights, sums them up and after that it applies the activation function to the sum. 
![alt text](https://github.com/kamleshak/NLP_Pytorch/blob/main/Neural%20Nets%20XOR/neuron1.png?raw=true)


### What is the use of the learning rate?
Learning Rate through Gradient descent:  Gradient descent is a procedure for minimizing a loss function to find weights essentially; we compute the partial derivatives of the loss function to give us the slope that tells us what direction to change each dimension of w to get closer to the minima. Mathematically, we want to iterate on this equation below (where eta is the learning rate):

![alt text](https://github.com/kamleshak/NLP_Pytorch/blob/main/Neural%20Nets%20XOR/Learning_rate.png?raw=true)

Thus from above equation we can say that learning rate governs the rate of convergence of gradient descent, thus to high learning rate may tend to drastic updates and give divergent behaviours, where as small learning rates may take longer duration to converge and sometimes may get stuck in local minima.

### How are weights initialized?
Weights Initialization:  In neural network weights could be initialized by any value and once gradient descent is able to reach its minima, final weights will get updated. However this is not the best way to initialize the weights, as any random weights may lead to lot of epochs for gradient descent to reach its minimum loss. Some of the best ways to initiate the weights are with truncated normal distribution. The truncated normal distribution is better for the parameters to be close to 0, and it's better to keep the parameters close to 0.  

![alt text](https://github.com/kamleshak/NLP_Pytorch/blob/main/Neural%20Nets%20XOR/weights.png?raw=true)

Three reasons to keep the parameters small:
1.	Experience shows that trained NNs often have small weights.
2.	Smaller weights lead to less extreme outputs (in classification, less extreme probabilities), which is desirable for an untrained model.
3.	It’s a known property of prediction models that adding a component to the loss function, which prefers small weights, often helps to get a higher prediction performance. This approach is also known as regularization or weight decay in non-Bayesian NNs.

### What is "loss" in a neural network?
Loss in NN: The Loss Function is one of the important components of Neural Networks. Loss is nothing but a prediction error of Neural Net. Let’s say actual value of wind speed in regression problem is 25 units and predicted value is 23 units so an error of 2 units.
 And the method to calculate the loss is called Loss Function. In simple words, the Loss is used to calculate the gradients.

### What is the "chain rule" in gradient flow?
Chain Rule in Gradient Flow:  In Neural network we have multiple neurons or hidden layers and for each neuron we need to re calibrate the weights for minimizing the loss. In calculus we take derivatives to get minimized loss of gradient or slope of curve.
Chain Rule: Calculus formula for calculating the derivatives of functions using related functions whose derivatives are known. Thus with the chain rule we are able to update the weights in NN in other words we could say back propagation in Neural network.
Page 205, Deep Learning, 2016.

## References:
https://jameskle.com/writes/neural-networks-101

Books: 
Probabilistic Deep Learning: with Python, Keras and Tensorflow Probability

Page 205, Deep Learning, 2016.



