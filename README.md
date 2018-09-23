# Simple Image Classifier using CNN
Train 2000 Dog and Cat images to different CNN models and analyzing their accuracy 

Our setup: only 2000 training examples (1000 per class)
We will start from the following setup:

a machine with Keras, SciPy, PIL installed. If you have a NVIDIA GPU that you can use (and cuDNN installed), that's great, but since we are working with few images that isn't strictly necessary.
a training data directory and validation data directory containing one subdirectory per image class, filled with .png or .jpg images:
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
To acquire a few hundreds or thousands of training images belonging to the classes you are interested in, one possibility would be to use the Flickr API to download pictures matching a given tag, under a friendly license.

In our examples we will use two sets of pictures, which we got from Kaggle(https://www.kaggle.com/c/dogs-vs-cats/data): 1000 cats and 1000 dogs (although the original dataset had 12,500 cats and 12,500 dogs, we just took the first 1000 images for each class). We also use 400 additional samples from each class as validation data, to evaluate our models.

That is very few examples to learn from, for a classification problem that is far from simple. So this is a challenging machine learning problem, but it is also a realistic one: in a lot of real-world use cases, even small-scale data collection can be extremely expensive or sometimes near-impossible (e.g. in medical imaging). Being able to make the most out of very little data is a key skill of a competent data scientist.
