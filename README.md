## Project Overview 

Our objective is to predict hourly bike rentals to ensure supply can meet demand. 
<br>
In addition, we will investgate the following business problems: 

<ul> 
	<li>Is there a day of the week when bikes are rented more than others?</li>
	<li>Is there an hour when bikes are rented the most?</li>
	<li>Is there a season when bikes are rented more than others?</li>
	<li>Is there a temperature when the most bikes are rented? </li>
</ul>	

## Code & Resources
<b>Python Version: 3.7</b>
<br>
<b>Packages:</b> pandas, numpy, sklearn, matplotlib, seaborn, pandas_profiling, math
<br><br>
<b>Data:</b> The 'Seoul Bike Sharing' dataset was provided by <a href="https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand" target="_blank">UCI Archives</a>.

The dataset was comprised of 1 year worth of bike rentals containing the following attributes: 
<ul>
	<li>Date (Dec 2017 – Nov 2018)</li>
 	<li>Hour of Day </li>
 	<li>Number of bikes rented hourly (0 – 3,556) </li>
 	<li>Hourly Weather Conditions (temp, humidity, rain, snow, wind, etc.) </li>
 	<li>Seasons (Spring, Summer, Fall, Winter) </li>
 	<li>Holiday (Holiday/Non-Holiday)</li>
 	<li>Functional Day (Closed/Open)</li>
</ul>

## Data Science Project Framework
<ul>
	<li>Frame the business problem</li>
 	<li>Obtain the data</li>
	<li>Preprocessing</li>
  <li>Exploratory Data Analytics (EDA)</li>
  <li>Perform in-depth Analysis</li>
  <li>Communicate Results</li>
</ul>
 
## Model Building & Performance

I started by transforming the categorical variables into numeric variables. <br>
Then I also created train and tests sets with a test size of 25%.
<br><br>
For the first model I included all data points as features. We tried three algorithms (Random Forest, Linear Regression, Support Vector Machine) and determined Random Forest performed the best. 
<br><br>
Random Forest Outcomes:  <br>
&emsp; R Squared: 0.929 <br>
&emsp; RMSE: 168.621
<br><br>
From our first model we discovered temperature and hour of the day were the most importnat features. With this insight I discritized the temperature data and built a new model with this new data point. I tried the same three algorithms (Random Forest, Linear Regression, Support Vector Machine) and determined Random Forest performed the best. 
<br><br>
Random Forest Outcomes: <br>
&emsp; R Squared: 0.925 <br>
&emsp; RMSE: 173.585
