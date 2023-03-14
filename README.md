# MavenSlopeChallenge

About this project

This project aims to help skiers find their ideal destination using a Power BI dashboard based on a dataset containing information on ski resorts, 
including their location, price, season, slope difficulty, lift types, and child friendliness.

Key Insights
- The snowfall distribution info can be used to help skiers to avoid booking trips during periods of low snowfall.
- By analyzing the breakdown of slopes by difficulty level, resorts are best suited for beginners, intermediate, and advanced skiers and snowboarders are being analyzed.
- Analyzed the distribution of ski resorts across different countries and continents thus skiers could also consider travel time and other incurred costs.

Data Preperation
- A few data transformation have been performed using Power Query and DAX.
- Snow Latitude and Longitude: combined both fields and concate with key words "Lat" and "Lon" to create a new calculated column "Snow Region"
- Resort Latitude and Longitude: categorized and determine which "Snow Region" the resort is located in, by rounding them to the nearest snow lat and long, and then concat with the same key words "Lat" and "Lon" .
- Available Seasons: transformed month name into month number by adding "01" for day, "2023" for year so that the data can be recognised as date. Get the month number in between and created a new table, related with resorts table by [ID], then further format the date to fulfil the needs to present a logical order in slicer.
- Ski Level: determined by calculating the percentage of beginner/ intermediate/ difficult slopes over total sloeps in a resort.

Data Visualization
- Considering the main task of this project is to help skiers to find their ideal destination, the visual is designed more like a travel website than a dashboard.
- 4 slicers are provided at the very top of the page, they are "When", "Where", "Ski Level" and "Price". These are all basic elements that viewers might already have in mind when they started to plan for a ski trip.
- A list of resorts are shown on the lower right, filtered by viewers' choices from the slicers above. Viewer can then click on each resort to get further details.
- Resort details are shown on the lower left, including opening seasons, type of slope in a horizontal bar chart, average snow time, price, and other resort features.
- Rsort pictures are also being used, skiers could have a more accurate expectation of the resort with an image.

More Possible Discoveries
- By analyzing the relationship between the cost of a ski pass and the length of slopes at each resort, we can identify which resorts offer the best value for money in terms of ski area.
- Identify the ski resorts that offer the best overall experience by considering factors such as price, length of season, length of slopes, and lift capacity.
