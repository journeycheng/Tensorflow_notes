# Tensorflow_notes

### 一、安装

- MAC

[Mac](./tensorflow_setup_note.md)

- Ubuntu 14.04LTS
    
    - pip
    ```linux
    $ sudo apt-get install python-pip python-dev python-setuptools build-essential
    $ sudo pip install --upgrade pip
    $ sudo pip install --upgrade virtualenv
    ```
    - tensorflow, CPU only
    
    ```linux
    $ sudo pip install https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.5.0-cp27-none-linux_x86_64.whl
    ```
 

### 二、模型及实践

- [1.notMNIST](notMNIST.ipynb)
- [2.Softmax模型推导](Softmax_model.ipynb)
- [3.举例分析FP和BP](FP_BP.ipynb)
