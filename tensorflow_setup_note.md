### 1.1 安装
- Mac OS X
```linux
$ pip install tensorflow
```

- 基于Docker
```linux
$ docker run -it b.gcr.io/tensorflow/tensorflow
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
