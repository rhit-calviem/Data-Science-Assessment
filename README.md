# Data-Science-Assessment
First Part of the Code: Locating and Storing Food Trucks

In the initial section of the code, we're focused on locating and storing information about local food trucks. We begin by importing the necessary libraries for data processing and mapping. An API key is used to access external services to retrieve data about food truck locations. In this case, we're using the Google Places API to search for food trucks within a specified area.

The code starts by defining the API key, latitude, longitude, and the keyword "food trucks" to identify these specific businesses. We then make API requests to obtain data about these food trucks, which includes their names, addresses, websites (if available), and opening hours. The retrieved data is stored in a DataFrame, which is a structured table-like format. This DataFrame is used to store the food truck information, which will later be saved in a CSV (Comma-Separated Values) file for further analysis and reference.

Second Part of the Code: Creating a Foodie Plan and Map

In the second part of the code, we use the previously obtained food truck data to plan a foodie experience and visualize it on a map. The foodie plan is organized into two days, with three food trucks selected for each day. A "Time" column is added to the plan, specifying the scheduled times for visiting each food truck. The travel distance and time to each food truck are calculated using the Haversine formula, with the assumption of an average driving speed. These calculations result in "Travel Distance" (in miles) and "Travel Time" (in minutes) values.

Based on the travel time, we determine the "Transportation Type" for each route. If the travel time is less than 5 minutes, it's assumed that attendees can walk to the food truck, so "Walk" is indicated; otherwise, "Car" is used for longer distances. The "Cuisine" information is excluded from the foodie plan, as per your request, to simplify the plan.

The foodie plan is then saved in a CSV file, named "foodie_plan.csv," for easy access and reference. Additionally, we create an interactive map using Folium to visualize the locations of the selected food trucks and the routes between them. This map includes markers for each food truck, and it visually displays the route following streets. The map is saved as an HTML file named "foodie_route.html."

In summary, the code accomplishes two main tasks: gathering and organizing data about food trucks for reference, and creating a two-day foodie plan with associated travel information that is visually presented on an interactive map. The foodie plan includes times, food truck names, addresses, travel distances, travel times, and transportation types. The map allows participants to visualize the route and locations for a delightful foodie experience.
