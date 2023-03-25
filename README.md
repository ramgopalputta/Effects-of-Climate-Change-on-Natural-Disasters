# Abstract of the project: 

Climate change has created a series of adverse effects on our planet. Is it causing an effect on the frequency and severity of natural disasters across the globe? 
If so, can governments save human lives and money by reducing climate change causes? Our carbon footprint harms the environment we live in as it is one of the main 
causes of human-induced climate change. As of October 11, 2022, there have been 15 weather/climate disaster events with losses exceeding $1 billion each to affect 
the United States (Billion-Dollar Weather and Climate Disasters, 2022). This study investigates the impact of CO2 emissions on the frequency and severity of natural 
disasters and questions whether it is possible for the US to save taxpayer dollars in mitigating the effects of these catastrophes. 
We find similar trends between global CO2 emissions, the count of natural disasters in the US, people affected by natural disasters in the US, and money spent on 
natural disaster relief by the US. Together, these trends indicate the possibility to improve US citizens’ lives and save the US government billions of dollars by 
working together with countries worldwide to reduce the CO2 emissions.

# Data cleaning and tools used:
Once the data is loaded into the coding notebook, the data from various data files are converted into data 
frame formats and comprehensive data preparation is initiated. The column names were renamed to have 
consistent field names, removed all the null values for considered columns, filtered out the required data, 
converted required data frames from wide to long formats, changed the data types, and dropped 
unwanted columns. Aggregation operations are performed over required columns to calculate the mean 
and median values. Considering the huge size of the data files, we narrowed our focus to specifically 
required columns for the disaster data set. For the disaster data set, we only used the columns which 
provided information about the number of deaths and those affected by each disaster.
After the data preparation is performed, a statistical visualization python library, ‘Altair’ is implemented 
to visualize the required plots. A series of world maps, bar plots, and line graphs are created to 
communicate the trends and data findings. We also used our knowledge of Tableau, a visual analytics 
platform, to create some of the visualizations which seem to be complicated using python libraries. The 
same data files were used as a source in this software to produce the charts in separate sheets and finally 
layered them together on a dashboard to extract as a static visual image

# Results and discussions:

***CO2 Emissions: The Global Trend:***

To investigate whether CO2 emissions impact the frequency or severity of natural disasters, we will first 
look at global trends in CO2 emissions. Fig 1 shows CO2 emissions in metric tons per capita in 2021 for the 
top 15 countries. It is important to note the US is among the top CO2 emitters. 

![image](https://user-images.githubusercontent.com/114395443/227745652-909b08a1-87fe-44b0-9b2a-4072b96fce35.png)

To get a better sense of yearly CO2 emissions, we show CO2 emissions in metric tons per capita for a 
select few countries for each year from 1960 to 2020. Countries were chosen to show a range of CO2 
emitters. In addition, we selected countries that are interesting to compare to the US such as China and 
India. Most importantly, we include a dotted line representing the global median emissions each year. 
This upward trending dotted line indicates that over time, CO2 emissions have been increasing worldwide. 
What we would like to do next is compare this trend to the occurrence of natural disasters in the US.

![image](https://user-images.githubusercontent.com/114395443/227745820-a8099c1e-9b41-4783-99b7-4531d0928b82.png)

***The Human Cost: Frequency and Severity of Natural Disasters***
Fig 3 shows us an upward trend in the count of disasters over time in the US. It is important to note, Fig 3 
shows us the counts of disasters from 1980 to 2022, while we can see from Fig 2 the upward trend in CO2 
emissions starts decades before this. Regardless, both trends are consistent even when focused on 
matching time periods. From this, there seems to be a strong relationship between global CO2 emissions 
and the frequency of natural disasters in the US. The largest attributor to the count of natural disasters 
over time in the US are severe storms. We can compare the counts of natural disasters to the counts of
other types of natural disasters as well.

![image](https://user-images.githubusercontent.com/114395443/227745847-beceb508-2fcb-40a2-8293-5a494034cf1f.png)

Before we look deeper at the severity of natural disasters in the US, we want to look at the global 
landscape. We chose to show the average of the past two decades to gather a more recent picture of 
global values. Fig 4 shows the total number of people affected per million in each country from 1998 to 
2018. It is observed that the USA is one of the most affected countries in the world, since the color of 
USA is towards the ‘red’ color shade of the color scheme.

![image](https://user-images.githubusercontent.com/114395443/227745869-88bbf437-954f-4773-a8b2-93e1ddf181fa.png)

Now, we will shift from looking at the frequency of natural disasters to their severity over time. Fig 5 
shows the top 5 countries with the most people affected by natural disasters in the most recent two 
decades. While the number for countries like China and India are five to ten times more than the US, the 
people affected in the US is still among the top 5 in the world.

![image](https://user-images.githubusercontent.com/114395443/227745888-019dd121-414f-4168-9664-9ba12ca034a3.png)

Next, we will look at how the severity of natural disasters has changed over time. We compare global 
trends to the trends in the US. Fig 6 shows yearly totals of people affected by natural disasters globally 
and for the US. Both show us increasing trends in people affected over time.

![image](https://user-images.githubusercontent.com/114395443/227745901-fe4ad44a-1221-41c7-8e89-9a2739e77dbe.png)

Fig 7 shows yearly totals of deaths by natural disasters globally and for the US. There does not appear to 
be any trend, however there are periods of time where natural disasters are more deadly. This likely has 
to do with factors such as population density of locations of the natural disasters and the degree of 
severity of the natural disaster.

![image](https://user-images.githubusercontent.com/114395443/227745917-d9fae8fb-14e4-4a0c-96f7-133f84f652e5.png)

In Fig 8A and 8B, we can compare which types of disasters affect the most people and cause the most 
deaths globally and in the US. In the US, storms are the major cause of people affected and death totals. 
This is corroborated by the trends we found in Fig 3 with the increasing counts of disasters in the US over 
time being attributed mostly due to the increasing counts in severe storms.

![image](https://user-images.githubusercontent.com/114395443/227745934-f09f5df1-e4ef-491f-9b84-cfe88e05f86a.png)

![image](https://user-images.githubusercontent.com/114395443/227745943-4bde5861-d6e6-4a8c-bfac-8cc7413a7f04.png)

Overall, we see the frequency and severity of natural disasters increasing over time in the US. We believe 
this trend is related to the upward trend of global CO2 emissions found before. Therefore, there is 
potential to save lives and improve outcomes for hundreds of thousands of people in the US and millions 
of people around the world if the world can reverse the trend of global CO2 emissions.

***The Monetary Cost: How much is the US spending?***

Now, we switch our focus to how much the US is spending due to natural disasters and whether this has 
any relation to CO2 emissions. During this analysis, it is important to note we are only considering disasters 
that cost the US over a billion dollars, CPI adjusted. We had this limitation due to the data collected. 
However, this likely will not affect the outcomes of the analysis due to the magnitude of the costs of 
disasters.
As we noted before a disparity between types of natural disasters in the US, we will first look at the trends 
of dollars spent per disaster type from 1980 to 2022. In fig 9, we can see the trends of the cost of each 
disaster type during this time period. Although severe storms account for the highest count of disasters 
in the US, the type of disaster that can be the costliest are tropical cyclones. Costs of disasters highly 
depend on the individual disasters and their degree of severity.

![image](https://user-images.githubusercontent.com/114395443/227745983-b46503e8-800f-4620-abd6-5b764170e57b.png)

We would like to compare the trend lines of median global CO2 emissions and cost of disasters in the US. 
Fig 10 shows us that both are increasing trends. There are significant fluctuations in the cost of disasters 
depending on the year. This is due to the individual severities of disasters occurring during those years. 
Despite this, the overall trend of the cost of disasters in the US is increasing.

![image](https://user-images.githubusercontent.com/114395443/227745997-ee84d20d-12d4-4873-83cf-617f83acdd43.png)

Fig 11 explicitly shows the trend of cost of natural disasters in the US per unit of CO2 emissions globally. 
This trend line shows that over time the cost of CO2 emissions regarding damage from natural disasters 
has increased. We do have fluctuations in the cost per unit of CO2 emissions, but overall, the increasing 
trend is worrying.

![image](https://user-images.githubusercontent.com/114395443/227746030-c9fd71a8-b350-4f08-9abc-d2a034e4c296.png)

This analysis shows the potential to decrease the financial cost of natural disastersin the US by decreasing 
global CO2 emissions. As such, it is in the United States’ best interest to work together with countries 
across the planet to reduce CO2 emissions.



# Conclusions drawn:
Climate change has many effects on our planet. This research focuses on climate change’s effect on the  human and monetary costs of natural disasters. Studies have shown that human-induced climate change is in large part due to CO2 emissions across the globe. Our analysis starts by showing the increasing global  trend in CO2 emissions. An increasing trend can also be seen for the counts of natural disasters, the number of people affected by natural disasters, and the cost of natural disasters across the United States. As such, it is possible that climate change causes these increasing trends of human and financial costs to the US. If countries around the world worked together to decrease human-induced climate change, our analysis shows it is possible to save and improve people’s lives and save the US government billions of dollars. 
In the future, we will need more information to establish a causal relationship between climate change and these increasing trends. There are three areas to focus efforts on. Further analysis of how people are affected by disasters is necessary. More detail is needed on how US dollars have been used for disaster events over time. Finally, consideration is needed of how data collection might have changed over time due to improved technologies on detecting natural disasters, obtaining numbers of people affected from disasters, and dollar values of relief efforts.

