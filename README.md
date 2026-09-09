# Weather-Generator
An app that generates weather based on Koppen Climate classification.

Refer to this post (https://42ducktape.blogspot.com/2026/09/weather-generation-redux.html) for an outline of the generator.

To use the app, download the HTML file, and just open in your preffered browser of choice (tested in Chrome and Edge)

The Generator is composed of 2 main sections: specifying the desired climate conditions, and inputting details of weather from the day before.

Select desired climate type, climate types are based on the Köppen climate classification system which is explained here: https://en.wikipedia.org/wiki/K%C3%B6ppen_climate_classification

Select the desired month(the generator uses the standard western calendar of 12 months, January to December), hemisphere(default is northern, if southern is selected the generator will just shift the month used to genrate the results by 6 months - July becomes January, etc), and number of days to generate weather for. The number of days ranges from 1 to 35, so you can have just on day or the entire month(35 is to account for fantasy calendars, e.g. the fantasy calendar I use for my D&D game has a max of 33 days in one of the months)

Select the base wind strength and direction, both of which will not depend on climate but on specific local conditions you are simulating. The "normal" wind strength setting can be imagined as the what might occur on the open ocean(it is based on the wind strength table from the 1981 edition of the D&D Expert set on pg X64), wind strength on land is generally weaker, though in large flat plains or deserts or high on mountains the wind strength might be stronger. The dominant wind direction will generally be determined by Latitude, but may be influenced by the local topography such as mountains or hills. The generator is set so there is a 44.45% chance of the dominant wind direction occurring, and a progressively less chance of other wind directions occurring as they get further from the dominant direction, so if the dominant direction is north, there is only a 5.56% of the wind being from the south

Starting Conditions are defaulted to random, but can be set to account for the weather from a previous day. The weather results for each day are affected by the conditions of the previous day, so if it is cloudy one day it will likely be cloudy the next, and the same applies to temperature and wind conditions and precipitation. Each climate type has a separate table for generating weather for each month, so if all the weather is generated for January, you can take the last entry from the last day of January and input the conditions to effect what the weather will be on the first day of February. 
