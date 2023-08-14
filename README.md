
<h1 align="center">Traffic Sign Classification Notebook</h1>

<p align="center">
  <img src=".\headline.png">
</p>

---

<p align="center">💡Python notebooks to create classification models of traffic sign images with CNN.</p>

## Table of Contents
* [General Info](#general-information)
* [System Requirements](#system-requirements)
* [Setup](#setup)
* [Usage](#usage)
* [Room for Improvement](#room-for-improvement)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## General Info
These notebooks creates classification models of traffic sign images. The models are created using Convolutional Neural Network (CNN) with Keras library. Dataset used in these notebooks is German Traffic Sign Recognition Benchmark (GTSRB). Created models used in [Traffic Sign Classification Web App](https://github.com/FlourCake/Traffic-Sign-Classification). By default, the models are trained using an RGB dataset with an image of size 128 x 128.

The default models created in these notebooks is a CNN model with 4 types of architecture (VGG16, ResNet50, InceptionV3, and Xception), and 2 types of image enhancement (Gaussian-blur, Sharpen, and Clahe). In the last, do manual parameter tuning with 2 types of batch size (32 and 64), and 2 types of learning rate (0.001 and 0.0001). The model will be saved in `[enhancement type]-model` folder.
| Architecture |    | Image Enhancement |    | Batch Size |    | Learning Rate |
|--------------|----|-------------------|----|------------|----|---------------|
| VGG-16       |    | Gaussian-blur     |    | 32         |    | 0.001         |
| ResNet-50    |    | Sharpen           |    | 64         |    | 0.0001        |
| Inception-V3 |    | Clahe             |
| Xception     |

## System Requirements
__Minimum:__
I don't know minimum system requirements for this project, but atleast you have 8 GB memory. Make sure you don't explode your computer.

__Recommended:__
The specifications below was used in this project:
|           |                                |
|-----------|--------------------------------|
| Processor | Intel core i5-10300H ~2.50GHz  |
| VGA       | Nvidia GeForce GTX 1650 TI 4GB |
| Memory    | 16 GB                          |
| Storage   | Atleast 5 GB for this project  |

With the specifications above, it takes about __5 hours__ to train 4 models with no image enhancement.

## Setup
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
* Open python notebooks on [Google Colab](https://colab.research.google.com/) or on your local computer with [Jupyter notebook __(Recommended)__](https://jupyter.org/install).
* Download the required dataset on [Acknowledgements](#acknowledgements). It is highly recommended to use `GTSRB_Online-Test-Images-Sorted.zip` as test data
* Extract datasets in the same folder as project folder.

## Usage
* Run `convert.ipynb` for `image_dataset_from_directory()`. You can ignore it if you use other data loader method eg. `data_generator()`.
* Run `split.ipynb` to enhance image data. You can ignore it if you use other data loader method that includes image enhancement.
* Run `train.ipynb` to train your models. __Beware don't run all in one if your computer doesn't meet the [System Requirements](#system-requirements)__. Also it takes a __long time__ to train the models.
* Run `score.ipynb` to get models test score. Models confusion matrix and models classification report will be saved in the same folder as models folder.

__Note:__
* Before running the notebooks, make sure you have the dataset in the same directory as the notebooks and change the dataset path in the notebooks.
* Run only necessary cell code.

## Room for Improvement
- Try using another method to improve performance.
- Increasing the epochs seems to improve performance (At the cost of increasing training time).

## Acknowledgements
> German Traffic Sign Recognition Benchmark (GTSRB) is one of the reliable datasets for testing and validating traffic sign classification and detection algorithms. GTSRB used in classification challenge held at the International Joint Conference on Neural Networks (IJCNN) 2011. Dataset has 43 classes with over 50.000 real-taken pictures.

__Dataset sources:__
You can download GTSRB dataset from official [INI Benchmark Website](http://benchmark.ini.rub.de/) or [Kaggle](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign).


## Contributing
Pull requests are welcome! If you see something you'd like to add, please do. For drastic changes, please open an issue first.

## Contact
Created by [Nolep Dev](mailto:support@nolep.web.id) - Feel free to contact us.

Copyright 2023 - Nolep Dev