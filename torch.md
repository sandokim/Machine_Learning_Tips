### torch.detach()

A simple and profound explanation is that use of with torch.no_grad() behaves just like a loop where everything written in it will have there requires_grad argument set as False although temporarily. So there is no need to specify anything beyond this if you need to stop the backpropagation from gradients of certain variables or functions.

However, torch.detach() simply detaches the variable from the gradient computation graph as the name suggests. But this is used when this specification has to be provided for a limited number of variables or functions for eg. ***generally while displaying the loss and accuracy outputs after an epoch ends in neural network training because at that moment, it only consumed resourced since its gradient won't matter in during the display of results.***
