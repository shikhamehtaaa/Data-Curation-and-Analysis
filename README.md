# Data-Curation-and-Analysis

The goal of my data curation and analysis project was to acquire data organizing cities around the world by their populations. After finding information about cities with high urban area populations, I intended to clean this data and convert it into a DataFrame. I aimed to create a DataFrame that effectively displays countries around the world according to their urban area populations. Finally, I worked to create various visualizations of my DataFrame to appropriately communicate the cities with the highest urban area populations and the disparity in population between some of the largest cities in the world.

I used an HTML parser in BeautifulSoup in order to scrape the website I found for data. Here's a link to BeautifulSoup documentation with some of BeautifulSoup's calls: https://beautiful-soup-4.readthedocs.io/en/latest/

The dataset I published has a public domain license because by publishing my dataset publicly on data.world, I am agreeing to relinquish all rights to it. My data source is PopulationStat (https://populationstat.com/cities/), specifically the table with the top 500 highest city populations. PopulationStat cites its source as World Bank. The World Bank makes its data available through a Creative Commons Attribution 4.0, or a CC-BY license. Finally, the license for my repository is an MIT License, so this license greatly reduces limits on reusing the code I publish in this repository. 

The attributes of my data are rank, city, country, urban area population, and city population. The rank attribute orders the 500 cities in the data from highest to lowest based on their urban area population. Rank comes in the form of an integer. The city attribute includes the names of the 500 cities in the table. This attribute is a text data type, specifically a string. The country attribute includes the names of countries that the included city is located in. Like the city attribute, the country attribute is a string. The urban area population attribute includes the amount of people in the general vicinity of the listed city, like the populations of surrounding suburbs in addition to the city. This attribute is an integer. However, the city population attribute includes strictly the amount of people in the listed city, excluding those living in nearby suburban or rural areas. The city population attribute is also an integer.

Some biases or misleading aspects of my data collection lie in the semantics of "urban area" compared to "city" and void data entries. Specifically, my data source, PopulationStat does not outline its definition of "urban area" compared to "city," so this may result in misleading information because some cities have suburbs that are extremely close to their urban centers. So, it is unclear how strict PopulationStat was in defining urban areas compared to cities. Additionally, city population data is frequently void, which may make it difficult for viewers to compare urban area population to city population for some cities. Also, it makes it difficult to get accurate descriptive statistics for city population.
