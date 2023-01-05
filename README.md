# AI4E_DL25: Waste Classification

Wastes are mostly defined as substances or objects which are no longer suited for their intended use. In order to protect our life, we find it important to work out what kind of material you have to deal with. Waste classification determines where you can dispose of waste material, how you must dispose of it, and whether you can sell the material on to be used at another site.

- We've been working on a solution for waste classification based on deep learning. 
- In this project, We separate three significant categories of domestic waste: recyclable waste (plastic, paper, glass-metal), biodegradable waste, and non-recyclable waste.

## Installation

Installing Python and dependencies
- [Python 3 and above](https://www.python.org/downloads/)
- OpenCV 3.4.0 for Python
- Numpy
- Keras
- Tensorflow
- Scikit-learn

## Dataset
The dataset includes 3495 images combined from selected data from [`Trashnet`](https://github.com/garythung/trashnet) and `Waste-set` (build by our own):
* Recyclable wastes:
    *  Plastic: 538
    * Paper/Cardboard: 616
    * Glass & Metal: 849
* Organic wastes: 487
* Non-recyclable wastes: 1005

You can download the dataset [here]()

![This is an image]()

## Data Augmentation
We use the ImageDataGenerator class1 from Keras to provide several transformations for generating new training data, such as rotation, zooming, translation, randomly flipping images horizontally, and filling new pixels with their nearest surround pixels.

## Experimental result
Model         | Accuracy
------------- | -------------
ResNet50  | 82.12
DenseNet121  | 83.26
SWIN | 88.26

## Usage

Clone the repository

```python
$ git clone https://github.com/maixbach/waste-classification.git
```


