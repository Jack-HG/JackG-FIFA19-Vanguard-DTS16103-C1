# JackG619-PROJECT-BRIEF-DTS16103-C1-Practical-Project-Report

What does the code do?

This project is a FIFA 19 database searching application. FIFA 19 is a video game based on real life football, which inludes real life players within the game. Each player has their own individual 'character' which has it's own statistics based on how the player performs in real life. For instance, statistics like sprint speed, agility, standing tackle, and finishing all based on their real life ability.

I retrieved all this information from an open source, in the form of a csv file. This code parses this csv file, processing the data and visualises the results. This answer specific questions, but also gives the user the ability to search through the 'database' to visualise data about their favourite players. FIFA 19 has different game modes, with information relating to the different game modes. This application seperates this information and can display it to the player.

For instance this application:
- has an introduction area - explains what the code does and what the can interact with
- has a 'menu' area - which allows the user to choose what they want to do within the applicaiton
- has a feature allowing the user to search the database. The user enters a player name they want to search for, the code then     returns which player's match this name. Allowing them to narrow down their search to avoid duplicates.
- can display the player's in-game statistics like sprint speed, agility, balance etc.
- can display information about the player like name, club, nationality, shirt number etc.
- can display career mode information like player monetary value, release clause value, potential rating etc.
- allows the player to specify a player, then specify which category of player they want to see. Then display the correlating       data the form of a radar chart. Visualising data in this way makes it much more readable.
- displays the top 20 players in the form of a bar chart
- gives an insight into the wages of players. With data analysis we can see visualisation of the correlation between wage and over rating and therefore perceived ability. Also correlation between wage and age.
- gives basic data analyis data analysis such as mean, range, mode values. Also the distribution of skill move and weak foot values.

This application also answer's the following questions:
- which player has the most total in-game stats? who is the most all round player?
- who are the top 100 players by overall rating?
- what is the correlation between wage and overall rating or age?
- what is the heaviest, lightest, tallest, shortest, oldest, youngest value of players?
- what is the distribution of weak foot and skill move values?

How do you use it?

The introduction and menu sections give brief explanations and pointers of how to use the application. Such as, prompting the player for an input, stating how this will direct them through the application. Or explaining which direction will allow them to do what. 

It is a text based program, so largely surrounds entering values such as 'yes' or 'no', or a certain number - both to signify what the user wants to do. Another input would be a player name, to specify which player's data you want to see.

Possible improvements and future features:
- When searching for some player's with accents, the database has trouble recongnising the name. For instance, the user may input 'Ibrahimovic' when the database entry is 'Ibrahimović'. So the code returns that the player was not found in the database, when in fact they are in the database. This can be worked around by just entering an abbrievated version, for example 'Ibra', and the full name would be returned. However, to improve this, some sort of unicode library feature would need to be implemented, to convert characters into their closest form, as unicode covers most characters.
- Implement a graphical user interface (GUI). This is because with text based applications it is hard to keep track of each element of a project, especially when user           interaction is involved. For example, having a numbered list, which requires the user to enter a number for what they want to do; which is complex and difficult to comprehend.   A GUI would allow me to implement a menu screen, that is user friendly and much more accessible. Clicking on a button would take the user to the desired path. This could also   allow for a drop down menu for player's, rather than having to input the exact name. Overall a GUI would be a welcome improvment to improve readability, accessibility and       make the program more user friendly.
- For the radar chart feature, an improvement would be to be able to compare two player's statistics on the same chart. Such as - https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.cs.middlebury.edu%2F~candrews%2Fshowcase%2Finfovis_techniques_s16%2Fradar_chart%2F&psig=AOvVaw1nn9vuaAskyVL4M5kcn020&ust=1601314130057000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCIC195XuiewCFQAAAAAdAAAAABAD - this would allow people to compare their favourite player's, meaning they could pick the better player.                   The visualisation of this comparison would make things much easier for the user.

CSV file and data source:
- Retrieved from open source - https://data.world/raghav333/fifa-players/workspace/project-summary?agentid=raghav333&datasetid=fifa-players 
- "FIFA PLAYERS dataset"
- "The dataset contains around 18000 fifa players scraped from sofifa.com"
- "It has over 88 features (columns)" 

References to libraries and open source resources:
- https://www.geeksforgeeks.org/python-pandas-dataframe/ - describes what a 'dataframe' is in the pandas library
- https://medium.com/python-in-plain-english/radar-chart-basics-with-pythons-matplotlib-ba9e002ddbcd
  https://python-graph-gallery.com/390-basic-radar-chart/ - both links offer guides to display radar chart information with the     use of the matplotlib library. These were used to adapt to this application.

Bibliography:
- https://pandas.pydata.org/docs/ - the pandas library documentation
- https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.pyplot.html - matplotlib.pyplot library documentation
- https://docs.python.org/3/library/math.html - math library documentation
- https://pandas.pydata.org/pandas-docs/version/0.23.4/generated/pandas.DataFrame.plot.html - used to gain knowledge on how to plot a bar chart
