# VRDL_HW4_README


Image Super Resolution

> This is the hw4 of Selected Topics in Visual Recognition using Deep Learning (2021).
> This homework, I use Mask RCNN to train the model.
## Installation

You can use conda to create a new virtual enrivonment.
And then install the [Pytorch](https://pytorch.org/) from the official webside.

For example:
```shell
$ conda create -n hw4 python=3.7
$ conda activate hw4
$ git clone 
$ cd VRDL_HW4
```


And then install the following packages

```shell 
$ pip install scikit-learn 
$ pip install pillow
$ pip install scikit-image
$ pip install tensorflow
```
---


## Data download and Prepare for training 
Please download the dataset from this [google drive  link](https://drive.google.com/file/d/1GL_Rh1N-WjrvF_-YOKOyvq0zrV6TF4hb/view) and put the files below to the data

![](https://i.imgur.com/zRCvclW.png)

And then run spilt.py to spilt the data to train and validation set




## Train the model
Now we are ready to train the model.

```shell
$ python train.py 
```
It will save the model to folder (/models)

## Run tensorboard 

```shell
$ tensorboard --logdir=./runs --bind_all
```



## test images and create the results 


We can run test.py to produce the results.

```shell
$ python submit.py
```

The results can be found in the folder output3

## Download models to reproduce the result

create the folder models
```shell
$ mkdir models 
```

Download the pretrain model from [here](https://drive.google.com/file/d/1-P1bD41MBMek9-5GliKLgdRCLcBvcrrU/view?usp=sharing) 

And put it in the folder models

And again, run the submit.py


## Reference 
- [pycococreator](https://github.com/waspinator/pycococreator)
- [detectron2](https://github.com/facebookresearch/detectron2)
