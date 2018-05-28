# Candy or Medicine Classifier
Could you tell the difference between candy and medicine? This python program is used to classify an image using TensorFlow with Inception v3 model to see if it is candy or medicine. 

## Prerequisites
- Python 3.5
- TensorFlow 1.5.0

## Approach
- Prepare a large dataset of candy and medicine for training purpose. Sample training images are available in tf_data folder
- The retrain script is retraining Inception V3 model, which is optimized for accuracy
- By running the retrain script, retrained_graph.pb which is a trained model and tf_files/retrained_labels.txt which is a text file containing Candy and Medicine labels will be generated. 
- Classifying an image

## Examples
#### An image of Medicine

```
python label_image.py predict/4076-8267-3450.jpg
```
![alt text](https://raw.githubusercontent.com/wingkwong/candy-or-medicine-classifier/master/predict/4076-8267-3450.jpg)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fwingkwong%2Fcandy-or-medicine-classifier.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fwingkwong%2Fcandy-or-medicine-classifier?ref=badge_shield)

```
Medicine (score = 0.98302)
Candy (score = 0.01698)
```

#### An image of Candy
```
python label_image.py predict/16394-2496-24495.jpg
```
![alt text](https://raw.githubusercontent.com/wingkwong/candy-or-medicine-classifier/master/predict/16394-2496-24495.jpg)

```
Candy (score = 0.99137)
Medicine (score = 0.00863)
```

## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fwingkwong%2Fcandy-or-medicine-classifier.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fwingkwong%2Fcandy-or-medicine-classifier?ref=badge_large)