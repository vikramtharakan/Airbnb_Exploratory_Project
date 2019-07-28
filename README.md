# Airbnb_Exploratory_Project
Used Airbnb data for Seattle and Boston across 2016/2017 to provide valuable insights into Airbnb usage

### Libraries Imported
requests <br>
from zipfile import ZipFile <br>
from os import path, getcwd, makedirs, listdir <br>
pandas <br>
numpy <br>
seaborn <br>
matplotlib.pyplot<br>
math <br>

from sklearn.linear_model import LinearRegression <br>
from sklearn.model_selection import train_test_split <br>
from sklearn.metrics import r2_score, mean_squared_error <br>


### Motivation
<p>
  In this project I took data directly from Airbnb's website for Seattle and Boston over 2 years to try and understand trends with the data. Specifically, I try and answer 3 questions:
  <ol>
    <li>How does the average number of booked bnb's fluctuate throughout the year?</li>
    <li>Were certain words used more often than others in the names of different bnbs? Were any words associated with higher ratings?</li>
    <li>Can we Predict the Pricing of different bnbs? What factors are the biggest indicators of price?</li>
  </ol>
