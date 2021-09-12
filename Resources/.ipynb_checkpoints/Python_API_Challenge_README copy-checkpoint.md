**# Python API Challenge**

1. Create a new repository for this project called `python-api-challenge`.  **\*\*Do not add this homework to an existing repository\*\***. - Done

2. Clone the new repository to your computer. - Done

3. Inside your local git repository, create a directory for both of the Python Challenges. Use a folder name that corresponds to the challenges, such as:  **\*\*WeatherPy\*\***.- Done

4. Inside the folder you just created, add new files called `WeatherPy.ipynb` and `VacationPy.ipynb`. These will be the main scripts to run for each analysis.-Done

5. Push the above changes to GitHub.-done

**### Adding A .gitignore File - Done**

Before we add our files to GitHub, let&#39;s add `api_keys.py` to the `.gitignore` file. Follow these steps:

1. Open your `python-api-challenge` GitHub folder in VS Code.

2. Open the `.gitignore` file, and on the first line type the following:

```python

# Adding config.py file.

api\_keys.py

```

3. While the `.gitignore` file is open, add the `API_practice.ipynb` and `random_numbers.ipynb` files and save the file.

4. In the command line, type `git status` and press Enter. The output should say the `.gitignore` file has been modified and the `WeatherPy.ipynb` file is untracked.

5. Use `git add`, `git commit`, and `git push` to commit the modifications to `.gitignore` and the `WeatherPy.ipynb` file to GitHub.

On GitHub, the only new file you should see is the `WeatherPy.ipynb` file.

**## Part I - WeatherPy**

I  created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized the following :

1 [simple Python library]([https://pypi.python.org/pypi/citipy](https://pypi.python.org/pypi/citipy))

2 the [OpenWeatherMap API]([https://openweathermap.org/api](https://openweathermap.org/api))

to create a representative model of weather across world cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

After each plot, add a sentence or two explaining what the code is analyzing.

\* Temperature (F) vs. Latitude

2021-07-28 15:57:07.088162
<img src = "images/max%20temp.png">

_ **This is a scatter plot for Latitude vs Max Temperature for all cities** _

2021-07-28 15:57:07.088162

<img src = "images/humid.png">

_ **This is a scatter plot for Latitude vs Humidity for all cities** _

\* Cloudiness (%) vs. Latitude

2021-07-28 15:57:07.088162

<img src = "images/cloud.png">

_ **This is a scatter plot for Latitude vs Cloudiness for all cities** _

\* Wind Speed (mph) vs. Latitude

2021-07-28 15:57:07.088162
<img src = "images/wind%20speed.png">

_ **This is a scatter plot for Latitude vs Wind Speed for all cities** _

The second requirement is to run linear regression on each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

\* Northern Hemisphere - Temperature (F) vs. Latitude

2021-07-28 15:57:07.088162

<img src = "images/NHtemp.png">

_This is a Linear Regression for Latitude vs Temperature for City of the Northern Hemisphere - Max Temp vs. Latitude Linear Regression_

This shows a negative correlation for Temperature as the Latitude goes up the Temperature goes down.

Based on this data I would say this does show a correlation between the 2

\* Southern Hemisphere - Temperature (F) vs. Latitude

2021-07-28 15:57:07.088162

<img src = "images/shtemp.png">

This is a Linear Regression for Latitude vs Temperature for City of the Southern Hemisphere - Max Temp vs. Latitude Linear Regression

This shows a Positive correlation for Temperature as the Latitude goes up the Temperature goes up. Based on this data I would say this does show a correlation between the 2

\* Northern Hemisphere - Humidity (%) vs. Latitude

2021-07-28 15:57:07.088162

<img src = "images/nhhumid.png">

This is a Northern Hemisphere - Humidity (%) vs. Latitude Linear Regression

This shows a slight positive correlation for Humidity as the Latitude goes up the Humidity goes up. Based on this data I would say this does not show much correlation

\* Southern Hemisphere - Humidity (%) vs. Latitude

2021-07-28 15:57:07.088162

<img src = "images/shhumid.png">

This is a Linear Regression for Southern Hemisphere - Humidity (%) vs. Latitude Linear Regression This shows a slight negative correlation for Humidity (%) as the Latitude goes down the cloudiness goes down. Based on this data I would say this does not show much correlation

\* Northern Hemisphere - Cloudiness (%) vs. Latitude

2021-07-28 15:57:07.088162

<img src = "images/nhcloud.png">

This is a Linear Regression for Northern Hemisphere - Cloudiness (%) vs. Latitude Linear Regression

This shows a slight negative correlation for Cloudiness (%) as the Latitude goes up the Cloudiness (%) goes down.

Based on this data I would say this really does not show much correlation

\* Southern Hemisphere - Cloudiness (%) vs. Latitude

2021-07-28 15:57:07.088162

<img src = "images/shcloud.png">

This is a Linear Regression for Southern Hemisphere - Cloudiness (%) vs. Latitude Linear Regression

This shows a slight positive correlation for Cloudiness as the Latitude goes down the cloudiness goes up.

Based on this data I would say this does not show much correlation

\* Northern Hemisphere - Wind Speed (mph) vs. Latitude

2021-07-28 15:57:07.088162

<img src = "images/nhwind.png">

This is a Linear Regression for Northern Hemisphere - Wind Speed (mph) vs. Latitude Linear Regression¶

This shows a flat or no correlation for Wind Speed as the Latitude goes.

Based on this data I would say this does not show any correlation

\* Southern Hemisphere - Wind Speed (mph) vs. Latitude

2021-07-28 15:57:07.088162
<img src = "images/shwind.png">

This is a Linear Regression for Southern Hemisphere - Wind Speed (mph) vs. Latitude Linear Regression

This shows a slight negative correlation for Wind Speed as the Latitude goes up the wind speed goes down.

Based on this data I would say this really does not show any correlation

After each pair of plots, take the time to explain what the linear regression is modeling. For example, describe any relationships you notice and any other analysis you may have.

final notebook must:

\* Randomly select  **\*\*at least\*\***  500 unique (non-repeat) cities based on latitude and longitude. - Done

\* Perform a weather check on each of the cities using a series of successive API calls. - Done

\* Include a print log of each city as it&#39;s being processed with the city number and city name. - Done

\* Save a CSV of all retrieved data and a PNG image for each scatter plot. - Done

As final considerations:

\* For Part I, you must include a written description of three observable trends based on the data. Done (see Below)

1. The 1st thing I observed is that as you go away from the equator the temperature gets colder.

2. wind speed and cloudiness really have no correlation to latitude It would be interesting to see if this change based on temperature and water temperature have a bigger impact on the 2 points.

3. Humidity have no correlation to latitude It would be interesting to see if this change based on temperature and water temperature I would think have a bigger impact on Humidity.

**### Part II - VacationPy**

Now let&#39;s weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.

To complete this part do the following:

\* Create a heat map that displays the humidity for every city from Part I.- Done
<img src = "images/heatmap.png">

\* Narrow down the DataFrame to find your ideal weather condition. For example:

  \* A max temperature lower than 80 degrees but higher than 70. - Done

  \* Wind speed less than 10 mph. - Done

  \* Zero cloudiness. - Done

  \* Drop any rows that don&#39;t contain all three conditions. You want to be sure the weather is ideal.

<img src = "images/hotel.png">

\* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates. - -done

\* Plot the hotels on top of the humidity heatmap with each pin containing the  **\*\*Hotel Name\*\*** ,  **\*\*City\*\*** , and  **\*\*Country\*\***. -Done

<img src = "images/hotel_map.png">

As final considerations:

\* You must complete your analysis using a Jupyter notebook. - Done

\* You must use the Matplotlib or Pandas plotting libraries. - Done

\* For Part II, you must include a screenshot of the heatmap you create and include it in your submission.
<img src = "images/heatmap.png">

\* You must use proper labeling of your plots, including aspects like: Plot Titles (with date of analysis) and Axes Labels. - Done

\* For max intensity in the heat map, try setting it to the highest humidity found in the data set. – Done