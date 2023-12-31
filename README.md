# MIST4610 Project 2
https://catalog.data.gov/dataset/baton-rouge-fire-incidents 

## Team Name:

15058, 15061 Group 1
## Team Members:

1. Jake Bogartz [@jab92323](https://github.com/jab92323)
2. Aiden Abramowitz [@aja1232](https://github.com/aja1232)
3. Max Young [@mxgyoung](https://github.com/mxgyoung)
4. Kiefer Sturisky [@ksturisky](https://github.com/ksturisky)

## Description of Dataset: 
Our dataset covers the emergency calls responded to by the Baton Rouge Fire Department. This dataset was found using the website https://catalog.data.gov/dataset. Our database contains a variety of data types. Examples of datatype number(whole) include Property Loss, Contents Loss, Fire Service Fatality, Fire Service Injury, Civilian Fatality, Civilian Injury, Property Value, Contents Value, Alarms, EMS Apparatus, EMS Personnel, etc. These data types contain whole numbers that describe each unique fire rescue mission. Our dataset also contains data string(VarChar) values such as Incident Number, Incident Description, Street Name, Formatted Street, City, State, Geolocation, etc. Finally, date/time data types are present in variables such as Dispatch Date, Dispatch Time, Control Date, Control Time, Clear Date, and Clear Time. Each one of the previous variables listed above describes individual fire rescues from the city of Baton Rouge.

## Question 1: 
In Baton Rouge, which zip codes had the most alarms triggered in the past year, excluding those with only 1 alarm? Based on the sum of alarms triggered per zip code, can determining the average fire control time reveal which zip codes need more fire rescue attention?

Importance: 
This question is important because it can identify alarm hot spots in the city of Baton Rouge. This can be extremely useful for fire rescue teams around the city for multiple reasons. First of all, the city of Baton Rouge can strategically place fire stations around the city based on where hotspots are located. This allows fire rescue teams to cut down on their response time. This is important because when rescue teams respond quickly, the damage would inevitably be reduced. In the cases of false alarms, with low response times, rescue teams would be able to take precaution and prepare themselves for the real cases. Also, finding alarm hot spots then leads to the question of why these areas have a higher number of alerts. Researchers can then focus on these areas in order to identify a cause and work towards a solution to lower the amount of alarms triggered.

<img width="996" alt="Screenshot 2023-12-06 at 9 41 07 PM" src="https://github.com/aja1232/4610-Project-2/assets/148247965/d1191397-477a-42f1-9ade-9330bde3f0c9">


The first graph shows a map of Baton Rouge by zip code. Each zip code shows the amount of alarms triggered, and is also color coded by the amount of alarm activity. The warmer colors represent higher activity, while the cooler colors show a lower amount of alarm activity. We noticed that a hot spot is located East of the river near downtown Baton Rouge. This also happens to be the location of the urban city. As the map spreads out into more rural areas we can see a decline in the amount of alarms triggered per zip code. In the next graph, we will look further in depth into the red zip codes to try and find out why this is the case. 

<img width="999" alt="Screenshot 2023-12-06 at 9 41 26 PM" src="https://github.com/aja1232/4610-Project-2/assets/148247965/dccbe7c9-efaf-4e71-b2ac-b61032c42118">


This second graph shows the average fire control time from each zip code that was depicted in graph 1. Here we can clearly see that there is an increase in average control time from zip code 70802 - 70810. What is interesting about this, is that the peak of this increase, 70808 - 70810, are not listed as hot zones in graph number one. This is most likely because the city has already tried to place fire stations near urban areas, therefore making the average control time of 70802 - 70807 slightly lower, while alarm count still remains high. We can then start to question if these zip codes with the highest control time need more attention in the future. However, the good news is that the more rural zip codes show a very low average control time, which could mean that they are getting the adequate amount of fire rescue attention. 

## Question 2: 
In Baton Rouge, which types of fire incidents cause the most civilian injuries? Does this data align with the incidents that also had the most suppression personnel on hand, or should priority shift?

Importance: 
	This question is important because it is dealing with civilian safety. By asking which incidents result in the most civilian injuries, fire rescue teams can know which kinds of incidents need the most attention. After establishing which fires need more attention, rescue teams can then allocate the correct amount of resources in order to prevent injuries. Ideally, suppression personnel is on site for every incident type, however, this may not always be available or necessary. This is why suppression personnel should prioritize high injury rate incidents. 

 <img width="999" alt="Screenshot 2023-12-06 at 9 41 51 PM" src="https://github.com/aja1232/4610-Project-2/assets/148247965/9f792493-be2c-4d7d-9f75-002066161a78">

 
In our first graph, we compared the sum of civilian injuries for each kind of incident. Instantly we knew that building fires were the main cause of injury. Even though this is a clear outlier, building fires are a very common incident and also a very general term that fire rescue teams use. This outlier is most likely due to the amount of building fire calls that occur in the city of Baton Rouge. All other incidents such as motor vehicle accidents, cooking fires, outside equipment, and other miscellaneous fires are fairly close in injury level. Even though these numbers were lower we wanted to make sure that these incidents were getting the correct amount of attention. After analyzing this data, the next question was to determine which incidents were being prioritized, and if those incidents aligned with the injury numbers. 

 <img width="1002" alt="Screenshot 2023-12-06 at 9 42 06 PM" src="https://github.com/aja1232/4610-Project-2/assets/148247965/76d8c03d-2ab3-4a62-989f-1428cfd96c20">


Our second graph shows the average number of suppression personnel at each individual incident type. In the right column you can see the averages of the personnel. The darker shades represent a higher average for that specific incident type. We wanted to be able to show which incidents were being prioritized. In this graph, we can see that building fires, cooking fires, and unintentional fires were among the incidents with the most personnel on average. This aligns with our previous graph which showed that building fires were by far the most responsible for civilian injuries. However, incidents like unintentional transmissions and smoke detector activation were not mentioned in the previous graph. While these incidents are precautionary measures, it might be worth noting that other events such as cooking fires may be of a higher level of concern due to their injury rate. Another thing to note is the extremely low percentage of assisting the EMS crew. This statistic could be useful when determining how to lower the amount of civilian injuries due to fires. It should also be very clear to all personnel that a building fire is to be prioritized and taken seriously at any point in time. 
 
## Manipulations:
There were no manipulations made to the data set. We did, however, have to regulate the data set. This means that we picked certain parts of the data and used it to answer the questions we came up with. The quantitative data we chose was all meaningful and important. There were some outliers we found in the data, but we only chose to include the meaningful data. The first question we used was comparing Baton Rouge zip codes to alarms triggered. When making the graphs for this, we excluded the data that only had one alarm. We did this by removing them from the data set. The purpose of this was to ensure that our analysis only focused on the significant patterns, which would therefore improve the relevance of our conclusions. We chose to do this to focus on the meaningful data. The second question we used was comparing the types of fire incidents and civilian injuries. Similarly to the first question, there were pieces of data we excluded for this as well. We removed all Incident Descriptions with less than 500 total Suppression personnel. The purpose of this was to make our findings more precise and insightful. By excluding this data, it is more likely that the chosen events had significant impacts on emergency response resources and the well-being of civilians. We chose to focus on events that would undoubtedly have greater consequences, making the conclusions more meaningful. 


## Tableau Packaged Workbook:

The tableau package workbook containing the graphs shown above is attached to this repository

