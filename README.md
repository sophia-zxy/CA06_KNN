# CA06_KNN
1. The Application

At scale, this would look like recommending products on Amazon, articles on Medium, movies on
Netflix, or videos on YouTube. Although, we can be certain they all use more efficient means of making
recommendations due to the enormous volume of data they process. However, we could replicate one of
these recommender systems on a smaller scale using what we have learned here in this article. Let us
build the core of a movies recommender system.

## Instructions
1. Open ipynb file
2. Click "Open in Colab" button or click the Colab link
3. Run code by lines or select runtime in the menu bar - click run all in the dropdown list

## Usage

import numpy as np

import matplotlib.pyplot as plt

import pandas as pd

from sklearn.metrics.pairwise import cosine_similarity

from sklearn.neighbors import KNeighborsClassifier

from sklearn.model_selection import train_test_split

from sklearn.preprocessing import StandardScaler

from scipy.sparse import csr_matrix

from sklearn.neighbors import NearestNeighbors

!pip install fuzzywuzzy

from fuzzywuzzy import process

## Questions answered

Given a movies data set, what are the 5 most similar movies to a movie query?
