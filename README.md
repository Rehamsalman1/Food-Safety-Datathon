# Food-Safety-Analysis - <a href="https://public.tableau.com/views/FoodSafetyAnalysis/DailyDashboard?:language=en-US&:display_count=n&:origin=viz_share_link">Link to the Dashboard</a>

## Transform data to create innovative solutions for a more sustainable food industry

With the world becoming more data-driven with endless amounts of data being collected from several sources, the Food industry has taken advantage of this to make significant decisions. Food safety has been a critical issue and a widespread interest has been growing on how to improve it to reduce its impact. The increasing use of IOT devices combined with big data analytics has played a major role in improving the food safety today. Furthermore, there are various benefits of leveraging the data to improve food safety and achieve good quality which are further illustrated in the report.

## Problem statement
Food safety is often overlooked in a company and we were presented with data from RUBICS Smart Solutions to help business owners be in more control of the food sustainability in the company. 

## Aim
The primary aim of our work is to present new innovative solutions and approaches that improve and enhance the quality of food produced today with the help of data provided collected from IOT devices used in the company.

## Original and Processed Data
Data collected from the IOT devices such as food temperature, fridge status, alert levels, location, and several other attributes were provided in the datatset to help create smart food insights for business owners and assist them in making quicker decisions. To leverage the data and achieve the proposed aim listed above the primary step was to clean the data and process it into meaningful insights. For our work we computed all our calculations and dashboards on Tableau. Originally excel limited the dataset to reach a certain number of rows for the Reading File thus giving a smaller dataset to work with on Tableau. However, to get a more real time analysis with updated data for comparisons we decided to manipulate the data and get all the data into excel through WordPad and later put it together by performing a union join to all the years Datasets into one source in Tableau. Thereafter, we moved to the next step of visualizing and creating dashboards to obtain meaningful insights.

# Analysis
After examining the data sets we made various visualizations and connected sheets to create dashboards acquiring valuable insights from the data which would further increase the Food Safety Quality and sustainability. Each of the visualizations is explained in detail below.

The devices often fail to record readings and miss out on valuable data that affects the food quality rate. This inaccurate data with missed readings inevitably results in the control department being unaware of any significant problems that may have affected the food in that time period. Additionally, with current analytics there has been little insight on the quality of devices which could be used as a key performance indicator to show if the device is reaching the expected quality rate over time. Thereafter, we decided to tackle these issues in our visualizations through dashboards which are illustrated below.

There are four key dashboards in this project; the first one summarizes the daily performance of the smart Food Safety Management system, while the device performance dashboard identifies the quality of each active device on a monthly basis. The "Available Devices Dashboard" shows the company’s devices along with the essential description of each device and where it is located in the factory. Finally, the last dashboard represents the temperature control chart of the selected device on a selected day.

## Daily Dasboard Tracker
 <img width="1024" alt="image" src="https://user-images.githubusercontent.com/42086991/174870317-1be39d42-b9f6-4ecf-ae52-50a577165801.png">
 
 The first dashboard is the Daily Analysis Dashboard that can be utilized to check the performance of the food system and analyze the metrics performance daily. Thus, solving any problem as it occurs , optimizing speed and alert performance throughout the business. There are filters on the dashboard that can be used to change the date to see daily reports of the filtered days.

### Dashboard Explanation
No of alerts: The first sheet on the dashboard is the Count of Alerts recorded in the day this information is significant as it shows the business if they had numerous alerts or if they performed well. Subsequently, they can drill down and trace the point that caused the alerts. These alerts are by several devices and they are broken down by the sheet “Alerts by Devices Sheet” that illustrates how many alerts are caused by each device. Consequently, aiding the manager to get a quick summarized view of which device had the most number of alerts and get the maintenance done faster to reduce errors later . 

The next sheet is the First Pass Yield% this sheet illustrates the percent of safe readings (readings that had Alert level Id 0) from all the devices in the Day. This yield% can depict how well the business in achieving safe readings and good alert-free food. 

Additionally, the third sheet shows the count of devices active on the day that is filtered. Furthermore, the alerts can also be seen as how many happened in the day and what percent happened in the night with the help of a pie chart. This would increase traceability for the business to quickly find the error at the specific time by drilling down into real time data and fix problems as they occur. 

Lastly, the sheet “Missed Readings” is crucial for daily performance to spot which devices have missed several readings and get the device inspected and fixed before the food spoils. All this information on one Dashboard gives the control manager a quick view to inspect on the daily metrics that are key and crucial to the business and any anomalies or outliers can quickly be identified. Thus, improving daily performance, traceability quality of food safety in the long run.

## Device Performance
<img width="1024" alt="image" src="https://user-images.githubusercontent.com/42086991/174870338-dbba38ec-c8fb-4fd0-b4da-b02d8236e59d.png">

The next dashboard that brings valuable key insights is the Device Performance Dashboard that focuses on providing a monthly analysis of devices to show the performance by month.

### Dashboard Explanation
 
The dashboard has filters that help the user to choose the specific month to see the performance of the device in that month. Each device sheet comprises of 2 sections the first describing the overall quality of the device in the selected month in which we created a calculated field( Quality of Device) that measures the number of normal readings then computes the percentage out of all the listed records. Each quality sheet has a reference line that holds the value of the expected quality rate of the device to be achieved that can be set by the business as a target (this value changes according to the client's requirements), and thus, the quality bar color helps the viewer understand if the goal was met or not. 

The bar color blue represents that a device has reached the expected potential and yellow depicts that the device has failed to reach the expected target that was set by the business. This gives a quick view to the manager to see if the device reaches the expected quality or not.
Identifying the quality percentage of the device can help the managers point out the devices that are not working as expected by the client, hence, helping them be motivated to achieve the expected target to improve the performance of the device.

However, the quality percentage cannot be the only factor that decides if a device is performing well or not since the amount of missed readings throughout the month plays a huge role in defining the quality as well. Therefore, we placed a sheet that outlines the daily count of missed readings by the device in the selected month. The MISSED READINGS calculated field counts the readings that were recorded in each day of the month and subtracts it from the total number of readings that is expected to be recorded by the device (since the expected time difference between each reading is 15 minutes, the total amount of records in a day is expected to be 96). A line chart was thought to be the most suitable graph type that will make the information more visually appealing. The user can interact with the dashboard to choose a different month of the year and check the performance of a device at the chosen time.
This alliance (the bar and line charts)would assist the system evaluator in understanding the functionality of the device from a wider perspective.

## Temperature Control Dashboard
<img width="1024" alt="image" src="https://user-images.githubusercontent.com/42086991/174870378-0dee8c79-d02d-4111-9200-65eb82bc3524.png">

Another dashboard that we thought is key for the business to gain valuable insights is the Temperature quality control chart. 

### Dashboard Explanation
This dashboard represents a real-time temperature analysis of the individual device where the chart has upper and lower control limits that are used as the minimum and maximum values assigned to the device. If the reading goes beyond the control limits specified, an alert would be sent to the manager.
This visualization is crucial to the food safety manager as it enables them to view the real-time temperature values and also go back to previous alert events to check how much time it took to respond and fix the issue.

Additionally, it helps in monitoring the food and making quick decisions to save the food whenever problems arise in the day. Consequently, the food recall rate would decrease, and the food is safer. Lastly, they can filter and choose the time that they want to inspect the temperature of the device.

## Available Devices Dashboard
The dashboard above represents all the food management devices available in the company and some details about the devices, including the name of each device, the group which they belong to, and where each device is located.

### Dashboard Explanation
 The data that makes up this dashboard is derived from the device, group, and location tables of the database. Looking at the resulting dashboard, we come to know that the company has 40 management devices distributed among the 3 locations. This interactive dashboard can be filtered by the location.
When the viewer clicks on one location, it acts like a filter and therefore, displays the total number of available devices in the chosen location. Additionally, the individual device name will show up if it is located at the selected spot. Having a more-visual representation of the available devices of the company is beneficial as it can help the business keep track of the number of devices and perhaps check if they have a lack of machines of certain group in one or more locations.
 
# Insights
It is believed that by using the visualizations presented above, the company can increase the level of food safety in businesses.
The company's smart devices can record and report the temperature values of the storage units, and thus, it is crucial to assure that such devices are doing their jobs effectively and as expected from the client. With the help of the device performance dashboard, the manager could accurately locate the error or the device that is not reading the temperature every 15 minutes. The quality of the food can therefore be improved .
The visualization of missed readings can provide insights to the control manager to see which device is not performing well and as expected and can get the maintenance of it checked as the problem is identified. Additionally, by looking at the amount of missed readings we believe that the company should do a deeper analysis on the device performance and maintain the device on a regular basis to check if it is functioning well and they should definitely have an automated data set to note the timing of the maintenance this would help to see if there is a lag between checking the device consequently improving the performance.
The quality rate that is used a reference line in the device performance dashboard can help the business reach the quality target and make them more government compliant and reduce the food recall rate. Consequently, improving their value and food safety .

# Conclusion
Food safety has been a topic for several years. However, recently with the help of Big data it has increased and improved the quality of food. The quality of device and checking the performance can amplify the effects on reducing the food wastage. Daily analysis and checking performance will translate into quicker responses to non-conformances and reduce inadequacies in storage and distribution leading to an overall increase in quality of food safety and higher value for the business. This data about the quality of food and devices can also be further then sent to government to show that they are following the government guidelines. Therefore, improving the value for the business.
