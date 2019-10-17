# Simple Image Classifier using CNN
Train 1000 Dog and 1000 Cat images to different types CNN architecture and analyzing their accuracy

### Setup: 
* Only 2000 training examples (1000 per class)
* A training data directory and validation data directory containing one subdirectory per image class, filled with .png or .jpg images:
```
data/
    train/
        dogs/
            dog001.jpg
            dog002.jpg
            ...
        cats/
            cat001.jpg
            cat002.jpg
            ...
    validation/
        dogs/
            dog001.jpg
            dog002.jpg
            ...
        cats/
            cat001.jpg
            cat002.jpg
            ...
```
### Image Source:
Kaggle(https://www.kaggle.com/c/dogs-vs-cats/data): 1000 cats and 1000 dogs(although the original dataset had 12,500 cats and 12,500 dogs, we just took the first 1000 images for each class). 
We also used 400 additional samples from each class as validation data, for model validation.
