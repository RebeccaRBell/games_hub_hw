## Task
Draw a diagram showing the dataflow through the application starting with a form submission, ending with the re-rendering of the page. This will involve a multi-direction data-flow with the client posting data to the server and the server sending data back to the client with the response. Detail the client, server and database in the diagram and include the names of the files involved in the process.



Questions
#### What is responsible for defining the routes of the games resource?

The create_route.js file within the helpers folder of the server creates the router function containing the various routes that will be applied to the routes when they're assigned/created in the server.js file. 

#### What do you notice about the folder structure? 

there are separate folders for front-end functionality and back-end functionality

#### Whats the client responsible for? Whats the server responsible for?

The client is responsible for hosting the front-end services, whilst the server is responsible for the back-end services.

#### What are the the responsibilities of server.js?

server.js is responsible for assigning the routers and running the servers

#### What are the responsibilities of the gamesRouter?

The gamesRouter has been assigned the gamesCollection and is an api for this data from the database 

#### What process does the the client (front-end) use to communicate with the server?

The client communicates with the server via a post method of a form located in the GameForm component and the GamesService file

#### What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs

The second parameter can be an object containing any custom settings that you want to apply to the request. In this application methods are added including post and delete.


#### Which of the games API routes does the front-end application consume (i.e. make requests to)?

the baseURL which is http://localhost:9000/api/games/

#### What are we using the MongoDB Driver for?

we are using the driver to access the data stored in the database whilst using javascript