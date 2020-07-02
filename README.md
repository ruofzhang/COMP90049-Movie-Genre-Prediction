# COMP90049-Movie-Genre-Prediction

The goal of this project is to build machine learning models to predict the genre of a movie based on its audio, visual and textual features. 

The data given in this project are derived from the ```MMTF-14K``` and ```MovieLens``` data sets, which is comprised of three parts: the training set (5240 instances), the validation set (299 instances), and the test set (298 instances). 

For each set, there are two files, one describes the features whereas the other one describes the genre labels. Each movie is labeled with a single genre from the following 18 possible ones: ```action```, ```adventure```, ```animation```, ```children```, ```comedy```, ```crime```, ```documentary```, ```drama```, ```fantasy```, ```film_noir```, ```horror```, ```musical```, ```mystery```, ```romance```, ```sci_fi```, ```thriller```, ```war``` and ```western```.

As for the features, except for the unique indices movieId and YTId that indicates the movie trailer’s URL, they can be generally divided into three categories: ```metadata features```, ```visual features``` and ```audio features```. 
Metadata features are textual fields that describe the title, year of release and tag of a movie; visual features and audio features are continuous ﬂoating point values extracted from the trailer of each movie. 

# Pre-processing of features

Feature pre-processing of this project mainly includes two parts: ```feature selection``` and ```transformation```. 

Features were selected based on three criteria: 

- assumptions based on daily life experience 
- statistical details
- techniques such as Principal component analysis (PCA) 

The transformation includes the matrix representation of the textual features and the discretization of the numerical features.

# Models and training

```Logistic Regression``` and ```Neural Network``` were used to build classification models in this project. The training stage mainly involved parameter tuning. ```GridSearchCV``` from scikit-learn was used to search for the best parameters.

#	Validation and testing

Validation and testing stages of this project includes the comparison between trained classifiers and baseline classifiers. Learning curves were drawn to diagnose the overfitting or underfitting problems.

Performance of the trained classifiers in validation and testing stages was presented and analyzed. Details can be found in report.pdf




