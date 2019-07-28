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
    <li>How does the average number of booked bnb's fluctuate throughout the year? How does it differ by city?</li>
    <li>Were certain words used more often than others in the names of different bnbs? Were any words associated with higher ratings or different prices?</li>
    <li>Can we Predict the Pricing of different bnbs? What factors are the biggest indicators of price?</li>
  </ol>
</p>

### Files in the Repository 
* boston.zip   --> Zip file containing data about bnbs from Boston. Acquired by scraping it off of Airbnb's webiste
* seattle.zip   --> Zip file containing data about bnbs from Seattle. Acquired by scraping it off of Airbnb's webiste
* boston_folder	--> csv files from boston.zip file. Had to keep in a separate folder from the seattle csv files because the files from both of these zip folders have the same name
* seattle_folder	--> csv files from seattle.zip file
* AirbnbProject.ipynb	  --> Notebook containing all cleaning and analysis work

### Summary of Analysis
<p> 
    For the first question we found that the number of booked bnbs actually did fluctuate quite a lot over the year. We also found that the most popular times to book a bnb depended on the city. For Boston the most popular time was the end of summer, specifically September, with the most booked day coming the day after labor day. On the other hand the most popular time for bookings in Seattle was January, with the most popular day coming after New Years. Both citie generally had less bookings in the winter months, besides the aforementioned spike for Seattle in January.
</p>
<p>
    The second question had us first find a list of the most popular buzz words used in the names of different Air bnbs, and then look at how their respecitve average price and rating differed. It was interesting to see that regardless of the city, bnb's that used the word "charming" in their title were very cheap while still maintaining an average to above average rating. I guess I'll look for airbnb's that use the word charming from now on, and if I ever rent out my place on airbnb, I'll make sure to use the word charming!
</p>
<p>
    The third question had us build and train a model on our data. This involved using both categorical and quantitative data, filling in missing values, and ultimately determining what factors had the biggest effect on price. There was definitely more work that could be done here to improve the r^2 value of .472, but I believe this is still a good model. The factors that had the biggest effect on price were "accomodates", "cleaning_fee", and "bedrooms".
</p>

### Acknowledgements
Thanks to Airbnb's website for providing the data for this research
