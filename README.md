# Airbnb_Exploratory_Project
Used Airbnb data for Seattle and Boston across 2016/2017 to provide valuable insights into Airbnb usage

### Libraries Imported
import requests
from io import BytesIO
from zipfile import ZipFile
from os import path, getcwd, makedirs, listdir 
import pandas as pd
import numpy as np
import seaborn as sb
import matplotlib.pyplot as plt
%matplotlib inline
import math

from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import r2_score, mean_squared_error

### 
