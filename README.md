
<h1 align="center">Traffic Sign Classification Notebook</h1>

<p align="center">
  <img src=".\headline.png">
</p>

---

<p align="center">💡A python notebook that creates classification models of traffic sign images with CNN.</p>

## Table of Contents
* [General Info](#general-information)
* [Usage](#usage)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## General Info
This notebook creates classification models of traffic sign images. The models are created using Convolutional Neural Network (CNN) with Keras library. Dataset used in this notebook is German Traffic Sign Recognition Benchmark (GTSRB). Created models used in [Traffic Sign Classification Web App](https://github.com/FlourCake/Traffic-Sign-Classification).

The default model created in this notebook is a CNN model with 4 types of architecture (VGG16, ResNet50, InceptionV3, and Xception), 4 types of batch size (8, 16, 32, and 64), and 2 types of learning rate (0.0001 and 0.001). The model will be saved in `model` folder.
| Architecture |    | Batch Size |    | Learning Rate |
|--------------|----|------------|----|---------------|
| VGG-16       |    | 8          |    | 0.001         |
| ResNet-50    |    | 16         |    | 0.0001        |
| Inception-V3 |    | 32         |
| Xception     |    | 64         |

## Usage
* Clone this repo
```bash
git clone https://github.com/FlourCake/Traffic-Sign-Classification-Notebook.git
```
* Go to project directory
```bash
cd Traffic-Sign-Classification-Notebook
```
* Install dependencies
```bash
pip i -r requirements.txt
```
* Open python notebook on [Google Colab](https://colab.research.google.com/) or on your local computer with [Jupyter notebook](https://jupyter.org/install).

__Note:__ Before running the notebook, make sure you have the dataset in the same directory as the notebook and change the dataset path in the notebook.

## Acknowledgements
> German Traffic Sign Recognition Benchmark (GTSRB) is one of the reliable datasets for testing and validating traffic sign classification and detection algorithms. GTSRB used in classification challenge held at the International Joint Conference on Neural Networks (IJCNN) 2011. Dataset has 43 classes with over 50000 real-taken pictures.

__Dataset sources:__
You can download GTSRB dataset from official [INI Benchmark Website](http://benchmark.ini.rub.de/) or [Kaggle](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign).

## Contact
Created by [Nolep Dev](mailto:azka.hisbullah26@gmail.com) - Feel free to contact us.

Copyright 2023 - Nolep Dev