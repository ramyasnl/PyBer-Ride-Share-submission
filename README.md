# PyBer-Ride-Share-submission<br/>
#**Overview of the analysis:**#<br/>
We are creating a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib,<br/> 
we are creating a multiple-line graph that shows the total weekly fares for each city type. <br/>
**Deliverable1:**<br/> We are creating a dataframe which classifies the cities according to their types and find the Total number of rides,Total number of drivers,<br/>
                Sum of Fares ,Average fair per ride,Average fares per Driver for the corresponding cities.<br/>
**Deliverable2:**<br/> We are creating a Matplotlib plot('fivethirtyeight') to analyse the datas by taking the "months" in X axis and "rates" in Y axis.<br/>
##**Steps involved**##<br/>
##**Deliverable1**##<br/>
Step 1: Read the csv files and create the corresponding dataframes "city_data_df" and "ride_data_df".<br/>
Srep 2: Merging the two DF s by the common column "city" we create "pyber_data_df"<br/>
Step 3: Classify the datas according to the city "types"<br/>
Step 4: Count all the values to create a new DF "pyber_summary_df" citiy,ride,driver,total_fares,average_fares per ride<br/>
Step 5: After cleaning it gives the DF<br/>
Image deliverable1<br/>
![mod5del1(2)](https://github.com/ramyasnl/PyBer-Ride-Share-submission/blob/main/mod5del1%20(2).png)
##**Deliverable2**##<br/>
Step 1:Renaming the columns,set index to date,Reducing the columns ["Fare","city","type"]<br/>
Step 2:Changing index to datetime.<br/>
Step 3:Creating new DF grouped by City type and date,Create a pivot table with index as ""date & column as "type "<br/>
![tablewithNas](https://github.com/ramyasnl/PyBer-Ride-Share-submission/blob/main/withNas.png)<br/>
Step 4:Using "loc" frome the above data we get pyber_pivot_df_weekly<br/>
![renaming](https://github.com/ramyasnl/PyBer-Ride-Share-submission/blob/main/resampledDF.png)<br/>
![pyber_challenge](https://github.com/ramyasnl/PyBer-Ride-Share-submission/blob/main/pyber_challenge.png)<br/>
#**Analysis**#
From the above plot we can say the Maximum Amount of Fare got collected in the month of February 24 on all the type of Cities.</br>
Also the minimun Fare got collected is different for all the city types ,for Rural its on Jan ,Suburbs its on March ,Urban its on Jan </br>
so the number of drivers may be increased on the second two weeks of february ,on all type of places so that Pyber can address more customers than regular days.
