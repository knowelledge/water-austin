# Water you building in Austin?

This project is trying to predict residential and commercial water consumption based on building permit data for Austin, TX. By understanding the relationship between metrics of urban development across city tract areas and water usage, resource management planning can be improved for future growth leading to efficiency gains. The impact will be better insight of what drives water demand as well as potential strategies for mitigating scaling aspects of those growing pains given limited resources.


## Background

* [Water Consumption Prediction](https://okavvada.github.io/Water_Consumption_Prediction/) - uses same water data from Austin's open portal but applies sophisticated spatialization techniques for estimating people by block reduced to ground level; not specifically predicting future consumption with data
* [Methodology for Evaluating Water Use in the Commercial, Institutional, and Industrial Sectors](http://www.waterrf.org/PublicReportLibrary/4375.pdf) - uses customer classification, explores alternative “rate-of-use” metrics; scope is much broader
* [Water resources long term planning framework](https://www.water.org.uk/policy/environment/water-resources) - UK drought mitigation for next 50 years


## Methodology

My approach is distinct by using building permit data to better predict future consumption. It bridges the gap between above analyses that use demographic and urban density data to predict water consumption by integrating a heuristic for those metrics that provides better insight for future estimations of demand.


## Presentation

As time permits:
•	Tier 1 - powerpoint slides
• Tier 2 - Visualization - matplotlib, Tableau or pygal / leaflet
•	Tier 3 - AWS or squarespace (wateraustin.org) - overview of project methodology, similar to github plus embedded visualizations
• Tier 4 - create ETL for automaticallly updating model, predictions and visualizations based on consistently updated data from Austin's open portal


## Data Sources

* [Residential Water Consumption] (https://data.austintexas.gov/Utilities-and-City-Services/Austin-Water-Residential-Water-Consumption/sxk7-7k6z) - 11k rows
* [Commercial Water Consumption] (https://data.austintexas.gov/Utilities-and-City-Services/Austin-Water-Commercial-Water-Consumption/5h9c-wmds) - 14k rows
* [Building Permits] (https://data.austintexas.gov/Building-and-Development/Issued-Construction-Permits/3syk-w9eu) - 403k rows of raw building permit data from 1921 to 2018; 40k building permit rows for 2018 alone updates as of 4-16-2018
* Storage format - postgreSQL database


## Potential Problems

Still need to do more exploration to really say but as of now it seems the feature engineering for creating the tract areas will be challenging. As well, the time series aspects of future predictions makes me a little weary. I think connecting the building permit data to actual growth and understanding the varied timeframes for how that affects water demand will be tricky.


## Next Steps

•	Solidify data sets and architect database
•	Understand how building permit data translates into development over time so as to apply analysis for future water prediction


## Built With

* [Python](https://docs.python.org/3/) - The programming language used
* [PostgreSQL](https://www.postgresql.org/) - Database Management

## Author

**Kelsey Nowell**

## Acknowledgments

* Hat tip to anyone who's code was used
* Inspiration
* etc
