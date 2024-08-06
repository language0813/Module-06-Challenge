# Module-6-Challenge

Instead of creating a file called "api_keys.py" to store my API key and adding that file to ".gitignore", I used the method taught in the class, which is to store API keys in the ".env" file. This method is easier and safer because the ".env" file was already included in the ".gitignore".

## WeatherPy

- Before creating a set of random latitude and longtitude combinations for the cities list, I set a random seed so the generated cities list is reproducible.

- Based on the OpenWeatherMap API document, I set the parameter "units" to metric for temperature in Celsius and wind speed in meter/sec.

- During the process of reading the saved city data CSV file, I noticed that the country code "NA" was read as "NaN". Therefore, I consulted ChatGPT how to fix this issue and was able to apply the method provided, successfully resolving the error.

- For the "Wind Speed vs. Latitude Linear Regression Plot" section, I wrote the entire syntax to create scatter plots instead of using the function created earlier. This was because the range of Wind Speed is much smaller than that of the other variables, making it difficult to position the annotation of the "line equation" correctly in all the plots. Althogh there might be a better solution, writing the entire syntax was the best approach I could think of at this point.

- Among the 559 randomly selected cities, the data cover almost the full range of latitudes, with 388 cities in the Northern Hemisphere and 171 cities in the Southern Hemisphere. The research could be improved by equalizing the number of cities in the Northern and Southern Hemispheres.

## VacationPy

- I narrowed down the "city_data_df" DataFrame based on my ideal weather conditions, which are maximum temperatures between 15 and 24 degree Celsius, 0% of cloudiness, and wind speed of less than 3 m/s. This narrowed down my list to 13 cities for later use.

- I successfully completed most of the requirements with what I learned in the class and the provided hints in the starter file. However, I encountered a trouble finsihing step 5. I used ChatGPT to look up the way to add addtioanl information to the hover message and was able to include the hotel name and the country by applying the method provided, which involves using the "hover_cols" parameter.

- I saved the two maps in HTML format in case they don't display in the main script because of the '%%capture --no-display' syntax that was included in the starter file.

## Resources

Resources that I referred to for completing this homework:

<https://chatgpt.com/>
