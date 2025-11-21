# MIST-group-project2
Juvenile salmon measured fork lengths collected from baited “minnow” traps in Campbell Creek, Alaska

59925 Group Project 2

## Team Members:
1. Morgan Lemmings @morganlemmings 
2. Melissa Tran @melissatran0 
3. Mahathi Bodhanapalli @mrb74060 
4. Jason Gol @jasongold3 
5. Clark Farrell @clarkfarrell2

## Description of dataset:
The database, “Juvenile salmon measured fork lengths collected from baited “minnow” traps in Campbell Creek, Alaska”, was obtained through the https://catalog.data.gov/dataset website. The publisher is the US Fish and Wildlife Service. There are 402 rows and 5 columns. The columns consists of: reach_id which identifies each individual fish, whereas the fork describes where specifically in the river the fish was found. The fork length describes the distance from the tip of the fish’s snout to the fork in its tail and the last column describes the species of the fish. In terms of data types, the dates are date type data, fork length is numerical, and the rest is categorical data.

## Question 1: 
What is the average fork length of Chinook vs. Coho salmon across all reaches, and how does it vary by fork (Main Stem, North Fork, South Fork)?

Importance: The average fork length is a strong indicator of fish health, growth rate, and habitat quality. By comparing these two species of salmon, we can identify species-specific habitat use within each fork of Campbell Creek. The different sizes across the Main Stem, North Forth, and South Fork can reveal which areas support growth faster and which areas may be less productive. Differences by location help agencies understand localized habitat conditions, such as food availability, water temperature, or flow differences. Understanding which forks produce larger salmon can guide management strategies that support long-term fishery sustainability. By using this data, we can sustain healthy salmon populations that ensure the continuation of traditional fishing practices and cultural heritage since salmon have a deep cultural significance for Indigenous communities residing in Alaska. 

<img width="630" height="400" alt="Image" src="https://github.com/user-attachments/assets/3714a909-5ee8-4806-9d75-fe5ccd5860ed" />

This chart shows how average fork length of salmon changes by month, species, and river fork location. The two species shown are chinook on the left and coho on the right. Each species has three locations which are Main Stem, North Fork, and South Fork. Within each location the bars show the average fork length for June, July, August, and in some cases September. In the Main Stem chinook are longest in June at about 80 cm then decrease through July and August. In the North Fork chinook show a similar pattern since June and July hold the smaller values with a small rebound in September. In the South Fork the smallest values occur in August while the largest values appear in September. Chinook in the South Fork also tend to be slightly longer in general than those in the North Fork. In the Main Stem coho are longest in June and decline each month through August. In the North Fork coho again start highest in June and steadily decrease into August and September. In the South Fork coho show a similar trend dropping from June to August then slightly rising in September. Fish are generally longest in June across almost every species and fork. Lengths usually decline as the summer progresses likely due to sampling of younger fish later in the season. Chinook have higher fork lengths in general than coho. The South Fork tends to show the smallest August values while September rebounds slightly.

<img width="450" height="320" alt="Image" src="https://github.com/user-attachments/assets/7ecab455-ee4e-4df7-8930-fdeefa92ad1f" />

<img width="450" height="320" alt="Image" src="https://github.com/user-attachments/assets/d98ca1c5-034b-4c52-ae61-a707f98fc761" />

<img width="450" height="320" alt="Image" src="https://github.com/user-attachments/assets/0d51260f-220d-4e53-a86e-091a2a550a17" />
  
The box-and-whisker plot displays how the average fork length varies across the different parts of the creek, varies by month, and by species type. Each reach is represented by a box, which shows the distribution of fork lengths for all salmonids captured at that location. The line inside each box where the shades of green split represents the median fork length, while the upper and lower edges of the box show the 25th and 75th percentiles. The whiskers extend to the minimum and maximum observed lengths, highlighting the overall range of fish sizes within each reach.

The graph showcases the range of lengths, with the bigger boxes representing wider distributions and smaller boxes representing narrower distributions. Overall, the difference in average fork lengths over different sections of the river reflects differences in food availability, water temperature, and other environmental conditions the vary across reaches.

<img width="574" height="288" alt="Image" src="https://github.com/user-attachments/assets/eece7cda-5888-4d03-9f97-d133aafcb396" />


The heat map illustrates clear differences in fork length between species and across sampling forks and months. Once again shows that, Chinook salmon are consistently larger than Coho salmon, and both species show size variation depending on the fork where they were captured. The coloration on the heat map highlights how each species responds differently to specific forks, with certain locations producing noticeably larger or smaller fish. Additionally, seasonal diffrences are especially highlighted in this graph with Chinook showing their highest fork lengths in June, while Coho reach their largest sizes during June and July. Together, these patterns demonstrate how species, location, and time of season interact to influence fork length, which is effectively visualized through the color gradients of the heat map.



## Question 2: 
Can we predict the fork length of a salmonid based on the sampling reach and date of capture during the 2021 Campbell Creek study?

Importance: As stated above, fork length is a key indicator for understanding fish health, growth rate, and the quality of the habitat. Being able to predict fork length can reveal spatial and seasonal growth patterns. Predictive models will help identify habitats that produce faster-growing fish. Predictive models also help biologists anticipate when and where salmon will reach key size thresholds. Modeling growth over time will also aid in detecting shifts in timing, such as early or delayed seasonable development due to climate or flow changes. The data for fork length, species, date of capture, and sampling reach are once again the needed variables to answer the predictive analysis question. Reach represents spatial variation, while the date represents temporal variation, making them ideal predictors of growth.

<img width="630" height="400" alt="Image" src="https://github.com/user-attachments/assets/ec81bbed-753d-45f5-9ebe-2e6de07bef07" />


Analysis of the trend lines revealed several important growth patterns across reaches and species. Main Stem Coho and South Fork salmon (both Coho and Chinook) showed clear positive growth over time, while North Fork salmon exhibited little to no growth, with Coho remaining flat and Chinook declining. Main Stem Chinook also declined slightly, indicating mixed results within that reach. Overall, the South Fork emerged as the most consistent location for growth across both species, whereas the North Fork proved to be the weakest predictor, with flat or negative slopes. Species differences were also evident: Coho generally displayed stronger positive growth slopes than Chinook, whose growth was highly location-dependent, positive in the South Fork but negative in the Main Stem and North Fork. These regression equations can be used to predict fork length for any given day and reach. For example, on Day 20 in the South Fork, the predicted Coho fork length is approximately 58.1 mm, calculated as 0.44217×20+49.25


## Manipulations applied to the data set of analysis: 

To prepare the data for analysis, we first deleted any rows with missing fork length values in Excel so that only valid measurements were used in Tableau.

Question 1: Removing the null values from the fork length column improves the quality and reliability of the analysis because it ensures that only real measured lengths are used when Tableau calculates the averages. If null values had been left in the data they would not contribute any information but they could still affect how Tableau groups or counts the records. By taking them out you prevent the averages from being influenced by missing entries and you avoid situations where certain species or forks appear to have fewer or oddly skewed values simply because some observations had no recorded length. This makes the final chart more accurate since every bar represents only actual measured fork lengths and every comparison between species months and fork locations is based on complete usable data rather than a mixture of real numbers and missing measurements.

Question 2: The date field was set to a continuous format, which allowed us to create line charts and look at changes over time. Fork length values were averaged to reduce the impact of outliers and make comparisons clearer across different reaches and species. We grouped the data by both reach and species so that patterns could be visualized more easily. Trend lines were added to the line charts to show how fork length changed with date, and Tableau displayed the equations and R² values to measure how strong those relationships were. Finally, we used Tableau’s forecasting tool to project fork lengths beyond the study period, adjusting the forecast length and confidence intervals to fit the dataset.

