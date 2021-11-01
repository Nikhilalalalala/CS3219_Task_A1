### Submission for TASK A

#### How to run this project?
Ensure you have Docker and Docker-Compose installed and running. 
`cd TaskAFinal`
`docker-compose up`
`docker-compose build`
The project should be running now. 
You may access it by visiting http://localhost on your browser.

#### How is this project structured?
In this project, there is a folder reverse-proxy which is running on nginx. this server will direct any incoming requests to the relevant servers. 

* If one is trying to access the root path, they will be directed to the server named "server-home"
* If one is trying to access the path '\one', they will be directed to the server named "server-one"
* If one is trying to access the path '\two', they will be directed to the server named "server-two"

Each of these servers are a flask application with its own dockerfile and are separate containers. 
