# MNIST classification using RandOm Convolutional KErnel Transform (ROCKET)

In this repository, we use ROCKET to classify the MNIST dataset. ROCKET is CNN that uses random filters, the filters are not learnt, but randomly sampled without any  prior. more info [here](https://github.com/angus924/rocket) .



## Preprocessing

1. Flatten each image to be a vector of $784$ entries
2. Divide each the vector by $255.0$
3. z-normalize each vector



## Main dependencies

- numba $>= 0.51$
- scikit-learn $>= 0.23$
- seaborn $>= 0.11$

## Results

- ROCKET achieves $96\%$ accuracy using only $400$ random filters. 
- Probably this result can be increased by using more filters

## Conclusion
Although ROCKET is designed for time series classification, it is quite good at classifying images represented as time series of pixels. The most interesting finding here is that the performance is achieved using random filters, the number of learnable parameters in this network is nothing compared to deep neural networks built for image classification.
