<p align="center"><img align="center" src="https://raw.githubusercontent.com/Hidup-Sehat/.github/main/profile/Horizontal%20Logo-whitebg.png" alt="HidupSehat Logo"/></p>

# HidupSehat Machine Learning Model Development

In our app, there are 2 deep learning models and 1 machine learning model. Each model will be explained in each folder.

1. Our Object Detection model trained with a pre-trained model [SSD MobileNet V2 with FPN-Lite Feature Extractor 640x640](https://tfhub.dev/tensorflow/ssd_mobilenet_v2/fpnlite_640x640/1), shared box predictor and focal loss, trained on [COCO 2017](https://cocodataset.org/#home) dataset with training images scaled to 640x640. Then we Fine tuning with own and kaggle dataset, we set 40000 steps 64 batch on 7400+ images from 36 food classes.

2. Yoga Pose Detection we will use the [MoveNet Lightning](https://tfhub.dev/google/movenet/multipose/lightning/1) model, extract the keypoints and calculate the similarity between the user and the yoga image with [Euclidean distance](https://en.wikipedia.org/wiki/Euclidean_distance) on 8 different angles.

3. Recommendation based on user inputs in Diary feature on our app. From there we can recommend the feeds content, and calculate the words similarity using [Cosine Similarity](https://en.wikipedia.org/wiki/Cosine_similarity) and the [TF-IDF](https://en.wikipedia.org/wiki/Tf%E2%80%93idf) method.

4. Our Data Scraping on food nutrients sourced from [FatSecret](https://www.fatsecret.co.id/kalori-gizi/) and feeds content are from [HaloDoc](https://www.halodoc.com/artikel) using [BeautifulSoup](https://pypi.org/project/beautifulsoup4/)

# Library, Pre-Trained Model, & Method Used
* [TensorFlow](https://www.tensorflow.org/?hl=id)
* [TensorFlow SSD MobileNet v2 fpnlite 640x640](https://github.com/tensorflow/models/tree/master/research/object_detection)
* [TensorFlow Movenet Lightning](https://tfhub.dev/google/movenet/singlepose/lightning/)
* [Euclidean distance](https://en.wikipedia.org/wiki/Euclidean_distance)
* [Cosine Similarity](https://en.wikipedia.org/wiki/Cosine_similarity)
* [NLTK](https://www.nltk.org/)
* [Numpy](https://numpy.org/)
* [Pandas](https://pandas.pydata.org/)
* [Regex](https://regexr.com/)
* [TF-IDF](https://www.capitalone.com/tech/machine-learning/understanding-tf-idf/)
* [Scikit-learn](https://scikit-learn.org/stable/)
* [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
* [Matplotlib](https://matplotlib.org/)
* [difPy](https://pypi.org/project/difPy/)
* [PIL](https://pillow.readthedocs.io/en/stable/)
* [xml](https://docs.python.org/3/library/xml.etree.elementtree.html)
