# Question1
Question 1 Gradient Descent Project

Importance of gradient descent: It is a method which determines how well the machine learning model has performed given the different values of each parameter. In any model, we have the predicted results and the actual results. The difference between these two is known as the error. Imagine there was a mathematical function which represented the error. The objective is to always minimise this error function (so that our model can suitably represent the actual scenario) and often, calculus cannot find the answer to this. Gradient descent aids us in finding the minimum since it is an iterative optimisation algorithm.

Plain vanilla gradient descent: This is the simplest/unmodified form of gradient descent. It involves taking small steps toward the minima by utilising the gradient of the cost function. Imagine we had a valley and two hills on either side in a 2 dimensional setting. Plain vanilla gradient descent involves taking steps downhill toward the valley.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/Plain_vanilla_gradient_descent_loss_function.png?raw=true)

Momentum gradient descent: This is one of the modifications of gradient descent which was incorporated. It considers the past movements before going to the next step. While plain vanilla gradient descent is a man going down a hill slow and steady, momentum gradient descent is a heavy ball rolling down the hill. This means we barrel through ridges, small humps and local minima to reach the optimum. One can argue it brings out a "gravity effect" which propels us toward the optimum solution.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/momentum_Gradient_descent_lossfunction.png?raw=true)

Root Mean Square Propogation (RMSProp): Another modification which we incorporated. Works similarly to momentum but it takes a different approach. If we think of the heavy ball approaching the optimum, it can easily overshoot this because of the momentum it builds up. RMSProp makes use of an exponential average of the previous gradients before going to the next step. This means it uses a greater weight of the recent gradients before calculating its next step hence propelling itself faster towards the optimum.

Three hump camel function: Below is an illustration of the function we have chosen to illustrate gradient descent on. The function has three local minima and a shape valley.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/Three%20Hump%20Camel%20Function%20graph.png?raw=true)

Number of iterations:

![alt text](https://github.com/AML2019Group6/Question1/blob/master/Plain_vanilla_lossfunction_vs_numiter.png?raw=true)

![alt text](https://github.com/AML2019Group6/Question1/blob/master/momentum_lossfunction_vs_numiter.png?raw=true)



How results vary with step size:

![alt text](https://github.com/AML2019Group6/Question1/blob/master/Plain_vanilla_lossfunction_vs_stepsize.png?raw=true)

![alt text](https://github.com/AML2019Group6/Question1/blob/master/momentum_lossfunction_vs_stepsize.png?raw=true)

![alt text](https://github.com/AML2019Group6/Question1/blob/master/rmsprop_lossfunction_vs_stepsize.png?raw=true)


















![alt text](https://github.com/AML2019Group6/Question1/blob/master/rmsprop_Gradient_descent_lossfunction.png?raw=true)

![alt text](https://github.com/AML2019Group6/Question1/blob/master/rmsprop_lossfunction_vs_numiter.png?raw=true)


