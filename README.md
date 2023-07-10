# stein's-paradox
Suppose that I have a Gaussian distribution with a variance of unity and some mean which I don’t tell you. I then draw a single sample from this distribution, give it to you, and ask you to guess the mean. What do you do? Well, you don’t have a lot of information to go on here, so you just guess that the mean is the number I gave you. This is a good guess!

Now we play again, but this time, my distribution is a two-dimensional Gaussian. The covariance is the identity matrix (so this is equivalent to sampling from two independent one-dimensional Gaussians). But again I have not told you the mean (which is now a two-dimensional vector). Once more I draw a single sample from the distribution, hand it over to you, and ask you to guess the mean. You simply guess that the mean is the sample I have given you. Once more you have guessed well!

Now we do the same thing in three dimensions. I draw a single sample, hand it over to you, and ask you to guess the mean. Just as before, you guess that the mean is the sample I gave you. But this is no longer a good guess! Stein’s paradox is that if we play this game in three dimensions or more, a better guess is to say that the mean is this:

![image](https://github.com/sivak07/stein-s-paradox/assets/92813223/ec8ceed5-5b22-465e-be6c-db863869ad8b)

where D is the dimensionality of the Gaussian, and x is the sample drawn from the distribution. This is the so-called “James-Stein estimator." ![here](https://joe-antognini.github.io/machine-learning/steins-paradox)
