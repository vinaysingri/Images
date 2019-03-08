Name : Vinay Suresh

Batch : Batch-7

Email : vinay.singri@gmail.com

## 					Convolution 

Convolution in mathematics in basically a way of combining two functions to produce a third function.(g(x) = f(x) * h(x))

![alt](https://raw.githubusercontent.com/vinaysingri/Images/master/Convolution_of_box_signal_with_itself2.gif)

In terms of image processing convolution refers to the multiplication of 2 matrices,the original image pixel matrix and another matrix (called kernel).It is performed by sliding the kernel over the image matrix by one column or one row and mutiplying the values of both the matrices and adding them to get a single value.

![alt](https://raw.githubusercontent.com/vinaysingri/Images/master/convolution.jpg)

So the output will be reduced by ***m-1*** and ***n-1*** size where ***m,n*** is the size of the *kernel*.









##				Kernels/Filters

Kernel is a small matrix used for extracting features in convolution neural networks. It has many applications in image processing such as edge detection,blurring,sharpening.

As an example below are 2 kernels for detecting edges in X and Y directions of an image. 

![alt](https://raw.githubusercontent.com/vinaysingri/Images/master/xy_kernels.jpg)

This works on the logic that across the edges the intensities will be largely varied and by applying the above kernels captures the differences in respective directions.



Kernels/filters in CNN's are used to learn and apply such features helping in various image applications.





##				1x1 Convolution

A 1 x 1 convolution processes the input data cell by cell just mapping input cell with all its channels to an output cell without looking anything around.

​	![alt](https://raw.githubusercontent.com/vinaysingri/Images/master/1x1.gif)

It can be used in dimensionality reduction in the sense that an input image of say (7 x 7) with 30 features on convolution with 10 kernels of 1 x 1 will lead to the output size of 7 x 7 x 10.





##					Feature Map

When a convolution is applied to the input data using a kernel,the output produced is called as the feature map.

The given kernel is drawn accross the entire matrix of input data resulting in an output of feature map.

![alt](https://raw.githubusercontent.com/vinaysingri/Images/master/Feature%20Map.jpg)

CNNS's look for features such as vertical line,particular textures etc. and after every layer each of such features will be reported in feature maps.





## 									Activation Function

Activation function in neaural network converts an input signal of a node to an output signal, which is then fed as an input to the next layer in the network. The decision of what neurons to be fired in the next layer is taken by the output of the activation function of the previous layer.

ReLU is one of the activation functions used today which outputs a value if it is positive else it outputs 0.

![alt](https://raw.githubusercontent.com/vinaysingri/Images/master/relu.jpg)

