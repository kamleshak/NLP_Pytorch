
# Back Propogation in Neural Nets

Attempt is being made to understand the calculations of neural nets in excel. Small neural net is trained in excel.

Row in the image stands for EPOCH in NN.(considering only one example)
![alt text](https://github.com/kamleshak/NLP_Pytorch/blob/main/Back_Propogation/NN_Backprop.JPG?raw=true)

Above  mentioned image will give you details of various layers and calculation in Neural nets. From color coding we can see it is broadly distributed in to two halves, Feedforward and Backpropogation.
In Feedforward part we are able to compute the total error.Backpropogation is done with help of chain rules of partial derivatives.
From color code you can note thate partial derivatives computed in first row are used to update the weights in second row. This weights are updated as (w1-(learning_rate*computed derivative value))

## Learning Rate and Error.

![alt text](https://github.com/kamleshak/NLP_Pytorch/blob/main/Back_Propogation/Error_LR.JPG?raw=true)

From above plot we can infer that:

•	Error is seen reducing over the increment in each epochs.

•	With more learning learning rate our gradient is reduced faster with very less epochs intially, but eventually most of the gradients at various learning rates converge at the end. Note: As this is very simple example for illustration purpose it may not lead to any problem with higher learning rates.
