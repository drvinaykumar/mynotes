a smaller filter size in the first conv layer helps retain a lot of original pixel information in the input volume. A filtering of size 11x11 proved to be skipping a lot of relevant information, especially as this is the first conv layer.


DeConvNet

Notes: 1) stride is the amount by which a filter moves in number of pixels. 


Stacking all of these layers and adding huge numbers of filters has a computational and memory cost, as well as an increased chance of overfitting).


No use of fully connected layers! They use an average pool instead, to go from a 7x7x1024 volume to a 1x1x1024 volume. This saves a huge number of parameters.


