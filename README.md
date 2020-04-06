### Questions

1. What is responsible for defining the routes of the `games` resource?
	
	server.js line 18 - then ./helpers/create_router.js
	
2. What do you notice about the folder structure?  Whats the client responsible for? Whats the server responsible for?

	Client is responsible for requesting and rendering API data from the server (frontend)
	
	Server is responsible for sending API and data manipulation as requested from client (backend)

3. What are the the responsibilities of server.js?

	server.js holds database connection, creates and serves routes via running web server (express)

4. What are the responsibilities of the `gamesRouter`?

	gamesRouter takes in partial URLs passed from app.use and displays/manipulates appropriate information as requested

5. What process does the the client (front-end) use to communicate with the server?

	HTTP requests

6. What optional second argument does the `fetch` method take? And what is it used for in this application? Hint: See [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) on the MDN docs

	The 2nd argument in fetch is a paramater which allows it to take additional arguments, this allows us to narrow down the information requested

7. Which of the games API routes does the front-end application consume (i.e. make requests to)?

	http://localhost:3000/api/games/

8. What are we using the [MongoDB Driver](http://mongodb.github.io/node-mongodb-native/) for?

	The MongoDB Driver is used to convert language specific inputs to a generic type that the database can understand and utilize
