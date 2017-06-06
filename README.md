# Health
Interactive visualization of health in the United States using the CDC's 500 cities study (https://www.cdc.gov/500cities/). 

### Tools
I used d3.js, a JavaScript library to make the html, svg, and css based visualization interact directly with the data.
### Files
1. Clean data from CDC's 500 cities study.
2. 

### Problem Background
Health in the United States, especially with respect to health care, is a huge flashpoint in today’s national conversation. With the newly proposed Republican healthcare bill, coverage for people with pre-existing conditions is seriously threatened. Pre-existing conditions are now much more broadly defined, including many mental health problems, high cholesterol, high blood pressure, diabetes, cancer, COPD, and even asthma.
For this project, I wanted to gain insight into the prevalence of these conditions to get a sense of magnitude of impact these legislative changes might have on our country. The people with these conditions are hugely vulnerable to the final changes made to this bill, as it could make healthcare much more difficult and expensive for them. In order to set the full context necessary to understand this problem, I also explored the data the CDC collected on health insurance coverage across these cities. This allows the viewer to see the 

### Data Overview
The total population included in this data is over 103 million, just over one third of the United States population in 2014. Below is a list of the health outcomes, preventative measures, and unhealthy behaviors that are being measured in this study.
Specifically, I looked at percent of the adult population within each city with access to healthcare. I also calculated the standard deviation of lack of access between census tracts within each city to get a sense of the disparities within a city. 
Finally, I used the health conditions that are deemed to be pre-existing conditions under the newly proposed healthcare bill – as the people with these conditions are in an extremely vulnerable place in terms of their access to healthcare. I had played around with what the standard deviations, or disparities, in these health outcomes were within cities, but found that there was not much differentiation between cities and thus it was not terribly interesting to the story. The disparities between healthcare access, however, were drastic and thus are an important story to tell.

### Encoding Method
I decided to encode the data using longitude as the x-axis. As you can see below, health metrics such as physical health were not related to latitude in a meaningful way.
Buttons on the left allow you to highlight cities with particularly high or low levels of access to healthcare, so that you can follow them as they move across the y-axis. The transition component implemented allows you to follow the bubbles as they move, getting a sense of how given cities compare across these measures.

### So what?
My dynamic visualization allows insight into the prevalence of the different pre-existing conditions and the impact that this might have on people. In this data visualization it is possible to view disparity in terms of health care access. The viewer can also view this in terms of population size. The y-axis can be manipulated to show any number of pre-existing conditions because blood pressure and high cholesterol occur at a higher rate they were rescaled to fit. Color illustrates the percent rank of access to healthcare. The user also has the opportunity to highlight the top and bottom 10% in terms of access to healthcare. If the user mouse overs a bubble in the plot, these and more statistics are displayed as well as the city and state.  I considered linking this to a small map in a separate svg that would highlight to show actual location when mousing over a state; however, this would have required a significant amount of time to restructure my visualization. I believe this addition would be valuable in terms of providing a geographic hook for users viewing disparity of healthcare access across different locations. The users can also see longitudinal differences across the country. For example, between the Mid-West and the East Coast (e.g. Mississippi), citizens tended to suffer from comparatively worse health outcomes. This disparity, not only in healthcare outcomes, but across different geographic locations is revealing in that healthcare opportunities or forms of care might severely differ in terms of quality from location to location.  
