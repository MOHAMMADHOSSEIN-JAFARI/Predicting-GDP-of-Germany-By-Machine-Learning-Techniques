# Working-Project-Predicting-GDP-of-Germany-By-Machine-Learning-Techniques.
I have done the following activities. 
Importing the raw data of real GDP of countries as time series in Eviews.
	Getting the natural log of each country, and save it as a new time series with the name “l_name of country”, for example l_germany
	Running HP filter for the natural log of GDP of each country. As far as I understood we do the HP filter to extract the role of business cycles. The result of the HP filter is the potential GDP, which we need to calculate the output gap. During the calculation of HP filter, I set Lambda= 100 because our data is yearly. I saved HP- filter for each country with the name “hp_name of country” such as hp_germany
	Calculating the output gap for each country and save it. For example for Germany: 
	100* (l_germany - hp_germany)/ hp_germany and it is saved with the name germany_gap 
	Doing rolling window between output gap of Germany and out put gap of other countries to reach coefficients.  According to your recommendation, I set 10 as the length of the window, and because my data starts from 1970, I have the coefficients from 1979. I saved the time series with the name “ roll_country name”. For example, roll_spain. I extracted all the time series as excel files and combined them in a different excel file named roll. 
	I also calcuate the growth rate of GDP of Germany from 1979-2019. I will run Machine Learning techniques to predict Germany GDP growth rate as independent variable and the time-varying correlation coeficents- rolling correlations- as features. 
