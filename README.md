# Health
Interactive visualization of health in the United States using the CDC's 500 cities study (https://www.cdc.gov/500cities/). 
I used d3.js, a JavaScript library to make the html, svg, and css based visualization interact directly with the data.
The files included are: 
1. Data cleaning - pulling data directly from CDC's 500 cities study
2. Static visualization
3. Dynamic visualization


### Problem Background
Health in the United States, especially with respect to health care, is a huge flashpoint in today’s national conversation. With the newly proposed Republican healthcare bill, coverage for people with pre-existing conditions is seriously threatened. Pre-existing conditions are now much more broadly defined, including many mental health problems, high cholesterol, high blood pressure, diabetes, cancer, COPD, and even asthma.
For this project, I wanted to gain insight into the prevalence of these conditions to get a sense of magnitude of the impact these legislative changes might have on our country. In order to set the full context necessary to understand this problem, I also explored the data the CDC collected on health insurance coverage across these cities.

### Data Overview
The total population included in this data is over 103 million, just over one third of the United States population in 2014. The study measures the health outcomes, preventative measures, and unhealthy behaviors by percentage of population within a geographical area. These 
Specifically, I looked at percent of the adult population within each city with access to healthcare. I also calculated the standard deviation of lack of access between census tracts within each city to get a sense of the disparities within a city. 
Finally, I used the health conditions that are deemed to be pre-existing conditions under the newly proposed healthcare bill – as the people with these conditions are in an extremely vulnerable place in terms of their access to healthcare. I explored disparities across these health metrics within a city, using the standard deviation of the census tracts within each cityThe disparities in healthcare access within a city were drastic and thus are an important story to tell.

### Encoding Method
Each city is represented as a bubble, using longitude as the x-axis.
The size of each bubble shows, by default, the disparity of healthcare access within that city (SD of percent of population without access to healthcare of census tracts within a city). To see the population size of each city, simply click the "Population Size" button in the "Radius" section in the menu on the left.
The y-axis shows the percent of the population within each city afflicted with a given health condition. To see each health problem, simply click on the issue of interest in the "Pre-existing Conditions" menu on the left. The default is "Physical Health Issues".
The green and orange buttons on the bottom left, under "Access to Healthcare?", highlight the top and bottom 10% of cities by level of access to healthcare. You can follow them as they move across the y-axis. The transition component implemented allows you to follow the bubbles as they move, getting a sense of how given cities compare across these measures.

### So what?
My dynamic visualization allows insight into the prevalence of the different pre-existing conditions and the impact that this might have on people. In this data visualization it is possible to view disparity in terms of health care access. The viewer can also view this in terms of population size. The y-axis can be manipulated to show any number of pre-existing conditions because blood pressure and high cholesterol occur at a higher rate they were rescaled to fit. Color illustrates the percent rank of access to healthcare. The user also has the opportunity to highlight the top and bottom 10% in terms of access to healthcare. If the user mouse overs a bubble in the plot, these and more statistics are displayed as well as the city and state.  I considered linking this to a small map in a separate svg that would highlight to show actual location when mousing over a state; however, this would have required a significant amount of time to restructure my visualization. I believe this addition would be valuable in terms of providing a geographic hook for users viewing disparity of healthcare access across different locations. The users can also see longitudinal differences across the country. For example, between the Mid-West and the East Coast (e.g. Mississippi), citizens tended to suffer from comparatively worse health outcomes. This disparity, not only in healthcare outcomes, but across different geographic locations is revealing in that healthcare opportunities or forms of care might severely differ in terms of quality from location to location.  
