# Question1
Question 1 Gradient Descent Project

Three hump camel function: Below is an illustration of the function we have chosen to illustrate gradient descent on. The function has three local minima and a shape valley. 

![alt text](https://github.com/AML2019Group6/Question1/blob/master/Three%20Hump%20Camel%20Function%20graph.png?raw=true)

Importance of gradient descent: It is a method which determines how well the machine learning model has performed given the different values of each parameter. In any model, we have the predicted results and the actual results. The difference between these two is known as the error. Imagine there was a mathematical function which represented the error. The objective is to always minimise this error function (so that our model can suitably represent the actual scenario) and often, calculus cannot find the answer to this. Gradient descent aids us in finding the minimum since it is an iterative optimisation algorithm.

Plain vanilla gradient descent: This is the simplest/unmodified form of gradient descent. It involves taking small steps toward the minima by utilising the gradient of the cost function. Imagine we were on a hill and wanted to get to the bottom. Plain vanilla gradient descent involves taking steps downhill toward the valley. The following graph illustrates this.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/Plain_vanilla_gradient_descent_loss_function.png?raw=true)

Momentum gradient descent: This is one of the modifications of gradient descent which was incorporated. It considers the past movements before going to the next step. While plain vanilla gradient descent is a man going down a hill slow and steady, momentum gradient descent is a heavy ball rolling down the hill. This means we barrel through ridges, small humps and local minima to reach the optimum. The following graph shows how we manouver through these ridges so as to reach our optimum. We can observe that it is not the most natural of routes and eventually corrects itself at the end indicating momentum may not be the best for our function.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/momentum_Gradient_descent_lossfunction.png?raw=true)

Root Mean Square Propogation (RMSProp): Another modification which we incorporated. Works similarly to momentum but it takes a different approach. If we think of the heavy ball approaching the optimum, it can easily overshoot this because of the momentum it builds up. RMSProp makes use of an exponential average of the previous gradients before going to the next step. This means it uses a greater weight of the recent gradients before calculating its next step hence propelling itself faster towards the optimum. The following graph shows how smooth the gradient descent process is with RMSProp indicating it is really good for the function at hand.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/rmsprop_Gradient_descent_lossfunction.png?raw=true)

Number of iterations:
To start with, we utilised 10000 iterations in our code to visualise how many iterations it takes for our functions to converge to the optimum under each of the three variant of gradient descent. The first graph illustrates the plain vanilla loss function. We observe it takes very few iterations to converge.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/Plain_vanilla_lossfunction_vs_numiter.png?raw=true)

The second illustrates the momentum loss function. Again, it takes much less than 10000 iterations to converge.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/momentum_lossfunction_vs_numiter.png?raw=true)

Lastly, the RMSProp loss function which happens to take more iterations than the previous two cases, but once again it is much less than 10000.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/rmsprop_lossfunction_vs_numiter.png?raw=true)

How results vary with step size:
After reducing the number of steps to a much more sensible value of just 100 we get the following graphs.

![alt text](https://github.com/AML2019Group6/Question1/blob/master/Plain_vanilla_lossfunction_vs_stepsize.png?raw=true)

![alt text](https://github.com/AML2019Group6/Question1/blob/master/momentum_lossfunction_vs_stepsize.png?raw=true)

![alt text](https://github.com/AML2019Group6/Question1/blob/master/rmsprop_lossfunction_vs_stepsize.png?raw=true)

We can observe that the graphs for plain vanilla and momentum are quite similar in this case. A huge jump is seen before it reaches a point at which it converges. In the case of RMSProp, we can observe that there is a much more calculated and smoother approach towards reaching the optimum.

Although plain vanilla and momentum do appear to be more efficient in this case, if we had a more complex function such as the six humpcamel function, we would perhaps not have seen such efficiency from the two as opposed to RMSProp.

Overall, RMSProp is more reliable than the other two methods of gradient descent and should be employed over the two.


