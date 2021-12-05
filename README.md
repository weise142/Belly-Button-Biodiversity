# Belly-Button-Biodiversity
## Overview
The purpose of thi project is to create an interactive dashboard that allows users to explore the bacterial biodiversity that colonize human navels or belly button biodiversity. The dataset that was gathered reveals that a small handful of microbial species, also known as Operational Taxonomix Units(OTUs), were present in over 70% of people in the study, while the remaining microbial species found were relatively rare.
## Programs and Resources
- Link to my interactive dashboard: https://weise142.github.io/Belly-Button-Biodiversity/
- Link to the dataset: http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/
- Programs: D3, Plotly, Bootstrap, HTML, CSS, Javascript, VS Code
## Summary
1. Create a drop down menu and Demographics Panel: The first step was to add all of the ID numbers to the _Test Subject ID No_ dropdown so the user can select whichever ID they'd like from the dataset to view. This ID number is used to filter out the metadata pertaining to the selected ID number and store it in an object that is viewable on the webpage. I then used D3, a javascript library for manipulating data, to select the panel-body class from the foreach statement in my HTML file to iterate through the object and append the data to the demographics panel to show the proper information by ID number.

![This is an image](https://github.com/weise142/Belly-Button-Biodiversity/blob/main/drop%20down%20menu.PNG)

 2. Create a Horizontal Bar chart and Bubble Chart: The second step was to create a horizontal bar chart and bubble chart to show OTU information for that specific ID number. First I filtered the JSON data by the ID selected by the user, then created a trace for the chart with the top 10 sample values as the x and the OTU ID numbers as the y. Then I used Plotly to create the bar chart using this information. I then followed the same steps to create the bubble chart in the second picture:

 ![This is an image](https://github.com/weise142/Belly-Button-Biodiversity/blob/main/OTU.PNG)
 ![This is an image](https://github.com/weise142/Belly-Button-Biodiversity/blob/main/bubble%20graph.PNG)
 
 3. Create a Gauge Chart: The third step was to create a gauge chart. First I created my pie chart which has the gradient colors and labels that show from lowest to highest frequency washings per week. I then proceeded to created my needle by creating several SVG paths that would draw the neefdle and that correlates with the frequency of washing for the specific ID number. I then created a function that would use a switch statement to select the correct path drawing the needle depending on the belly button washing frequency. 

![This is an image](https://github.com/weise142/Belly-Button-Biodiversity/blob/main/Gauge.PNG)

4. Customize the Dashboard: In the fourth and final step, I customized the dashboard. In order to customize the dashboard, I added a picture to the header and changed the color of the lettering to make sure it contrasted with the picture and was able to be read, and adding a paragraph about the project to the website.
