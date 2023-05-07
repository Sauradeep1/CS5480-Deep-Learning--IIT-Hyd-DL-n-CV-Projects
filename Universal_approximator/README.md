Universal Approximation Theorem (2 + 2 + 1 + 1 + 2 = 8 marks) :
The Universal Approximation Theorem states (in simplistic terms) that for any continuous function
f : Rn → R, you can find a 1-hidden layer neural network that can approximate f to any
arbitrary precision on a closed interval. If you would like to know more about this theorem,
how it’s proved and what it intuitively means, please see this link for the original paper,
this link for some slides explaining the theorem, and this link for an intutive understanding
(highly recommended to read). What you will do now is to test this theorem programmatically.
(a) Consider the simple case of a function f : R → R, and write your code to implement
a 1-hidden layer neural network (with 1 input and 1 output, considering the function
considered - and say, 50 hidden neurons) with a ReLU activation function.
(b) Study the approximation capability of this implemented function to the well-known sine
function, f(x) = sin x. (Train your network using sine function as the ground truth).
What do you observe? You can use Matplotlib or equivalent to plot the original sine
function and the neural network approximation in a closed interval range.
(c) Try changing the number of hidden neurons, and see how the approximation behaves.
(Try reducing and increasing). Show your plots.
(d) What happens if you change the ReLU activation to sigmoid? Do you see any change
in convergence time taken?
(e) Take one more function of your choice (f(x) = x3, or f(x) = tan x, for example), and
study the same.
