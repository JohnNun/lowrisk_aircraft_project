# Low Risk Aircraft


## Business Understanding

The company is looking to expand into new industries to diversify its portfolio. They are primarily interested in purchasing and operating airplanes for commercial enterprises and want to investigate the potential risks of aircraft. With the use of the Aviation Accident data recorded by the National Transportation Safety Board, I will identify aircraft(s) that pose the lowest risk to the company.

## Data Understanding

The Aviation Accident data recorded by the National Transportation Safety Board, includes aviation accidents recorded from 1962 to 2023. This data contains records for civil aviation accidents and selected incidents in the United States as well as international waters for aerial vehicles ranging from gliders and balloons to jet planes for both commercial and military.

### Data Preparation

For Data Preparation and cleaning, I first create a new dataframe from the aviation data that contains the columns that may be the most beneficial. From there I normalize the column names and start dropping rows with values that do not fit the commercial plane criteria. 

Since the company wants to branch out to commercial aircraft, I did some research to find the leading companies for commercial aircraft. My research led me to two well-known and respected major aircraft manufacturers for commercial use, [Boeing](https://www.boeing.com/ 'Boeing website') and [Airbus](https://www.airbus.com/en 'Airbus Website). To narrow down the dataset to these two companies, I first double check if there are any company name variances in the dataset and then replace the variances with the respective company's commonly used name. After making names uniform, I created individual dataframes for Boeing, and Airbus to further clean their aircraft models to only show aircraft still in production by these companies. Finally, I combined the two dataframes and further dropped rows with null values that couldn't be filled with the data on-hand.


## Exploratory Data Analysis

#### Overall Data

Overall, the Boeing 737 holds the most records in the dataset, but that doesn’t necessarily mean that it is a high-risk aircraft as the 737 has been in production since 1967. Also, due to its popularity and reliability, it has been a highly sought-out aircraft since its first flight. The Airbus aircraft, namely the Airbus A220 first took flight in 2013, and since its creation, it appears only once in the dataset. That alone is enough to give this aircraft high praise for its safety and reliability.


#### Recorded Damge

The overall damage shows promising results with minor damage being the majority outcome for most of the aircraft present in the dataset, then followed by substantial damage, and destroyed.


#### Injury Severity

Like the damage to aircraft, the injury severity also shows a great overall outcome for these incidents where the best outcome in any kind of aircraft-related accidents is Non-Fatal. Unfortunately, the next outcome is Fatal, followed by Incidents. Despite the Boeing 737 holding the most records on this dataset, the majority and by a large margin is non-fatal, which speaks volumes towards the aircraft’s safety.


## Conclusion

The analysis of this data helps with answering the following questions to narrow down a low-risk aircraft.

**Which Aircraft has the highest damage severity overall?** 
The aircraft that holds the highest damage severity would be the Boeing 737, mainly due to its overwhelming number of records. If you were to compare records based off the damage outcome of the aircraft, then the Airbus A320 would have the highest severity as its destroyed outcome is almost equal to its minor damage outcome.

**Which aircraft holds the highest fatalities as compared to no fatalities?** 
By comparing the injury severity outcomes, the Airbus A320 holds the most fatalities based on its fatal to non-fatal ratio. The Boeing 737 on the other hand has a high non-fatal outcome compared to its fatal outcomes.

**Which Aircraft poses the lowest risk to the company to begin this new endeavor?** 
Of the recorded data, the Airbus A220 and A321-271N could be considered low-risk as these aircraft have only 1 recorded accident, which ended with minor damage to the aircraft, and no fatalities. As the oldest aircraft in the dataset, The Boeing 737 has an overwhelming data count compared to others, but this amount of data also works in its favor as a low-risk aircraft since most of the recorded damage is minor damage, and injury severity is majority non-fatal.

### Limitations

A major limitation with this dataset is that from the very beginning it contains a significant amount of null values or unknowns that could make the data be as accurate as possible. Another limitation from this dataset is that it only shows the recorded accidents these planes have experienced since thier first flight, and it doesn't exactly show the success flight rate for each aircraft.

### Recommendations

While the commercial aircraft has been narrowed down to 3, I believe further research and comparison of these aircraft is necessary to find out where each aircraft excels or falls short to ensure not only safety of the potential consumer, but for the success of the company in this field.

## Next Steps

Further analyzing the data could also give a better understanding of the safety of each aircraft, and how over the years the safety rating of each individual aircraft has advanced.

Also, exploring data that contains successful flight records either on a daily, weekly, or monthly basis for these aircraft can further help to identify a low-risk aircraft by comparing overall data of recorded accidents to overall successful flights.

If possible, getting record data of what the causes of these aircraft accidents can help further narrow down a low-risk aircraft. For example that kind of data could potentially give better insight on how well these aircraft operate in unpredictable weather, or if was system failures that caused these accidents, over human error.

