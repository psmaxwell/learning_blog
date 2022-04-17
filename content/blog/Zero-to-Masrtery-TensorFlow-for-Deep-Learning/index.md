title: Zero to Mastery TensorFlow for Deep Learning
date: "2021-07-14"
description:  "This course will teach us foundation of deep learning and TensorFlow as well as prepare you to pass the TensorFlow Developer Certification exam(optional)"



## 00.Getting started with TensorFlow: A guide to the fundamentals



### What is TensorFlow?

<font color=red>TensorFlow</font>  is an open-source end-to-end machine learning library for preporcessing data ,modelling data and serving models(getting them into the hands of others).





### Why use TensorFlow?

Because the TensorFlow contains many of the most common machine learning functions you'll want to use.



### What we're going to cover

TensorFlow is vast.But the main premise is simple: turn data into numbers(temsors) and build machine learning algorithms to find patterns in them.



we cover some of the most fundamental TensorFlow operations,more specificially:

- Introduction to tensors(creating tensors)
- Getting information from tensors(tensor attributes)
- Manipulating tensors(tensor operations)
- Tensors and NumPy
- Using @tf.function(a way to speed up your regular Python functions)
- Using GPUs with TensorFlow
- Excerises to try



### Introduction to Tensors

tensors are kinds of like NumPy arrarys ,you can think of a tensor as a multi-dimensional numerical representation of something. Where something can be almost anything you can imagine:

- using tensors oto represent the price of houses
- using tensors to represent the pixels of an image.
- using tensors to represent words.
- it could be some other form of information (or data ) you want represent with numbers.

The main difference between tensors and NumPy arrays(also an n-dimensional array of numbers) is that tensors can be used on GPUs( graphical processing units) and TPUs(tensor processing units).



The benefit of being able to run on GPUs and TPUs is faster computation,this means,if we wanted to find patterns in the numerical representations of our data,we can generally find them faster using GPUs and TPUs.

The first thing we'll do is import TensorFlow under the common alias `tf`.

In [ ]:

```
# Import TensorFlow
import tensorflow as tf
print(tf.__version__) # find the version number (should be 2.x+)
2.5.0
```

### Creating Tensors with `tf.constant()`

As mentioned before, in general, you usually won't create tensors yourself. This is because TensorFlow has modules built-in (such as [`tf.io`](https://www.tensorflow.org/api_docs/python/tf/io) and [`tf.data`](https://www.tensorflow.org/guide/data)) which are able to read your data sources and automatically convert them to tensors and then later on, neural network models will process these for us.

But for now, because we're getting familar with tensors themselves and how to manipulate them, we'll see how we can create them ourselves.

We'll begin by using [`tf.constant()`](https://www.tensorflow.org/api_docs/python/tf/constant).

In [ ]:

```
# Create a scalar (rank 0 tensor)
scalar = tf.constant(7)
scalar
```



A scalar is known as a rank 0 tensor. Because it has no dimensions (it's just a number).

In [ ]:

```
# Check the number of dimensions of a tensor (ndim stands for number of dimensions)
scalar.ndim
```

Out[ ]:

```
0
```

In [ ]:

```
# Create a vector (more than 0 dimensions)
vector = tf.constant([10, 10])
vector
```

Out[ ]:

```
<tf.Tensor: shape=(2,), dtype=int32, numpy=array([10, 10], dtype=int32)>
```

In [ ]:

```
# Check the number of dimensions of our vector tensor
vector.ndim
```

Out[ ]:

```
1
```

In [ ]:

```
# Create a matrix (more than 1 dimension)
matrix = tf.constant([[10, 7],
                      [7, 10]])
matrix
```

Out[ ]:

```
<tf.Tensor: shape=(2, 2), dtype=int32, numpy=
array([[10,  7],
       [ 7, 10]], dtype=int32)>
```

In [ ]:

```
matrix.ndim
```

Out[ ]:

```
2
```

By default, TensorFlow creates tensors with either an `int32` or `float32` datatype.

This is known as [32-bit precision](https://en.wikipedia.org/wiki/Precision_(computer_science) (the higher the number, the more precise the number, the more space it takes up on your computer).

In [ ]:

```
# Create another matrix and define the datatype
another_matrix = tf.constant([[10., 7.],
                              [3., 2.],
                              [8., 9.]], dtype=tf.float16) # specify the datatype with 'dtype'
another_matrix
```

Out[ ]:

```
<tf.Tensor: shape=(3, 2), dtype=float16, numpy=
array([[10.,  7.],
       [ 3.,  2.],
       [ 8.,  9.]], dtype=float16)>
```

In [ ]:

```
# Even though another_matrix contains more numbers, its dimensions stay the same
another_matrix.ndim
```

Out[ ]:

```
2
```

In [ ]:

```
# How about a tensor? (more than 2 dimensions, although, all of the above items are also technically tensors)
tensor = tf.constant([[[1, 2, 3],
                       [4, 5, 6]],
                      [[7, 8, 9],
                       [10, 11, 12]],
                      [[13, 14, 15],
                       [16, 17, 18]]])
tensor
```

Out[ ]:

```
<tf.Tensor: shape=(3, 2, 3), dtype=int32, numpy=
array([[[ 1,  2,  3],
        [ 4,  5,  6]],

       [[ 7,  8,  9],
        [10, 11, 12]],

       [[13, 14, 15],
        [16, 17, 18]]], dtype=int32)>
```

In [ ]:

```
tensor.ndim
```

Out[ ]:

```
3
```

This is known as a rank 3 tensor (3-dimensions), however a tensor can have an arbitrary (unlimited) amount of dimensions.

For example, you might turn a series of images into tensors with shape (224, 224, 3, 32), where:

- 224, 224 (the first 2 dimensions) are the height and width of the images in pixels.
- 3 is the number of colour channels of the image (red, green blue).
- 32 is the batch size (the number of images a neural network sees at any one time).

All of the above variables we've created are actually tensors. But you may also hear them referred to as their different names (the ones we gave them):

- **scalar**: a single number.
- **vector**: a number with direction (e.g. wind speed with direction).
- **matrix**: a 2-dimensional array of numbers.
- **tensor**: an n-dimensional arrary of numbers (where n can be any number, a 0-dimension tensor is a scalar, a 1-dimension tensor is a vector).

To add to the confusion, the terms matrix and tensor are often used interchangably.

Going forward since we're using TensorFlow, everything we refer to and use will be tensors.

