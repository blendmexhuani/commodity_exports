# Commodity exports per country

The topic selected for this project is *Country*, and we will try to answer the following question:

* ***How does the number of commodity exports per country relate to other country-specific parameters (e.g., population density)?***

The data used in this project comes from the following datasets:
1. [Global Commodity Trade Statistics](https://www.kaggle.com/unitednations/global-commodity-trade-statistics)
2. [World Development Indicators](https://databank.worldbank.org/source/world-development-indicators)

*Please note that in order for the notebooks to work properly, one needs to download and extract the data files given above. For more information, see data/README.md file.*

The first dataset comes from kaggle and it has a total of 207 countries with 10 attributes, and around 8.23milion rows. It contains data about import/export flow of commodity per country, for the years 1988–2016. Each record specifies the year, trade value (in US dollars), weight (in kilograms), quantity and category of the commodity. The second dataset comes from worldbank and has a total of 217 countries with 50 manually selected country-specific parameters, and around 6300 rows. These parameters mainly contain information about demographic and socio-economic status of the country, also for the years 1988–2016. Since both datasets contain information per country and for the same year span, later on we can use country and year attributes to merge these two datasets together.

Since the dataset from kaggle contains global trade statistics - from which we can analyze the flow of commodity exports - merging it with the data coming from worldbank, we end up with one huge dataset which will contain information about trading and other country-specific parameters. Using all that information, we can check correlations among different country statistics in order to determine how does the number of commodity exports (also imports) relate/correlate with other country-specific parameters. This will allow us to see if and in what amount the demographic and socio-economic status of the analyzed countries contribute in the trading of goods.

Here we will:

* Preprocess, parse and join the data (Wrangle) 
* Explore the data (Profile)
* Model the data
* Create an interactive dashboard