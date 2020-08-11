# reasearch-paper
# reasearch-paper


Overview
This application allows the user to fetch papers' abstracts related to current Computer Science research (like the Atom feed assignment). Once the user presses the button fetch, the application shows a list of available papers from a Web Service. If the user is further interested in one in particular, he/she could press the button "Learn More" to get more details and a link to the paper.
In order to keep the network usage low, my aim is that only the first time the button "fetch" is pressed the information will be downloaded. The rest of the time it will try to get info from the web service to see if local data is up to date, and only download only new data.
I will be updating the server with data each day with 1-2 paper information (or at least 7-10 per week), until the course is over. Beyond that point no new updates will be made on the server.

Android Application
The application will have a SQLite DB to store all the data. It will use the classes from the Atom feed examples to download new data from the web service. The list with the papers' information will be rendered in a RecyclerView, and the specific details of the chosen paper will be visible in the first half of the applicacion screen.
A link to the publicacion will be opened with an intent to a browser, for more interaction.

Web Service
The Web Service will keep a record of the last time it was updated. This will help the application known when it's time to fetch the new data.
