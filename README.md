## End-to-end Image Search engine

This is the end-to-end implementation of image search engine. The image search engines allow us to retrive similar images based on the query one.

## Project Instructions

### Getting Started

1. Clone the repository, and navigate to the downloaded folder.
```
git clone https://github.com/lucko515/image-search-engine
```

2. Install TensorFlow.
	- Option 1: __To install TensorFlow with GPU support__, follow [the guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.
	```
	pip install tensorflow-gpu==1.12.0
	```
	- Option 2: __To install TensorFlow with CPU support only__,
	```
	pip install tensorflow==1.12.0
	```

3. Install a few pip packages.
```
pip install -r requirements.txt
```

4. Download CIFAR-10 dataset.

	  - [Darknet mirror](https://pjreddie.com/projects/cifar-10-dataset-mirror/)
    ```
    1. Put downloaded data into dataset folder
    2. Put all images from `dataset/train` to `static/images`
    ```
    - [CIFAR-10 homepage](https://www.cs.toronto.edu/~kriz/cifar.html)
    
    ```
    1. Preprocessed the dataset (not covered here)
    2. Save each image in the jpg/png format into train/test folders
    3. Rest of the project stays the same
    ```


5. Run throuh [image-search project.ipynb](https://github.com/lucko515/image-search-engine/blob/master/image-search%20project.ipynb) and generate all necessary files

6. Start the app.py file and enjoy!

## Steps to improve the engine!

#### (1) Use color features as an additional search filters

We could use color intesity to produce additional features and improve our image search engine. Good read for this: [Pyimagesearch color histograms](https://www.pyimagesearch.com/2014/01/22/clever-girl-a-guide-to-utilizing-color-histograms-for-computer-vision-and-image-search-engines/)

#### (2) TensorFlow Serving pipeline version

The Flask approach works, but it is not scalable. If you want to create the system more scalable you will need to change the implementation to TensorFlow Serving.

#### (3) Use Hourglass attention mechanism

#### (4) Use pre-trained model
