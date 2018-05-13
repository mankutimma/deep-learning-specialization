It's a myth that cost decreases every iteration when you use BGD(or when minibatch_size=m) or any other optimizer which uses all 'm' examples for one iteration, 
even when forward_prop, initialize_parameters and the rest of the code is bug-free.

Decreasing cost depends on many things such as learning_rate, NN architecture, how well the data is pre-processed etc.,

The code in this directory("Tensorflow_Tutorial_Adam_Ashish.ipynb") is proof of what is stated above. 
NOTE: optimizer used is Adam and not BGD, but its ok since 'm' examples are processed for 1 iteration. 
	  Using BGD also causes cost to shoot up sometimes only if learning_rate is relatively larger than what was used for Adam.