# Tensorflow_notes

## 一、入门

### 1.1 安装
- Mac OS X
```linux
$ pip install tensorflow
```

- 基于Docker
```linux
$ docker run 0it b.gcr.io/tensorflow/tensorflow
```
该命令将启动一个已经安装好TensorFlow及相关依赖的容器。

### 1.2 安装测试
```python
>>> import tensorflow as tf
>>> hello = tf.constant('Hello, TensorFlow!')
>>> sess = tf.Session()
>>> print sess.run(hello)
Hello, TensorFlow!
>>> a = tf.constant(10)
>>> b = tf.constant(32)
>>> print sess.run(a+b)
42
```
### 1.3 基本用法

- 使用图（graph）来表示计算任务
- 在会话（Session）的上下文（context）中执行图
- 使用tensor表示数据
- 通过变量（Variable）维护状态
- 使用feed和fetch可以为任意（arbitrary operation）赋值或者从中获取数据

------

TensorFlow是一个编程系统，使用图来表示计算任务。图中的节点被称为op（operation的缩写）。一个op获得0个或多个Tensor，执行计算，产生0个或多个Tensor。每个Tensor是一个类型化的多维数组。

一个TensorFlow图描述了计算的过程。为了进行计算，图必须在会话里启动。会话将图的op分发到诸如CPU或GPU之类的设备上，同时提供执行op的方法。这些方法执行后，将产生的tensor返回。在Python中，返回的tensor是numpy ndarray对象。


