# Task 1

### Requirements

- Java
- Maven
- Spring Boot (Framework)
- MongoDB
- Docker

#### Dependencies

- spring-boot-starter-web
- spring-boot-starter-data-mongodb
- spring-boot-maven-plugin



## Rest  API Endpoints and Resources
Rest API Endpoint is mapped to `http://127.0.0.1:9090/servers/`

- PUT a server	`http://127.0.0.1:9090/servers/createServer`
Accept "server" object in body in json format.

- GET servers	`http://127.0.0.1:9090/servers/getServer`
Returns a list of "server" objects.

- GET server	by ID	`http://127.0.0.1:9090/servers/getServer?id=<ID>`
Returns a  "server" object matching with ID.

- GET servers	by Name	`http://127.0.0.1:9090/servers/getServer?name=<Nmae>`
Returns a list of "server" objects matching with Name.

- DELETE server	`http://127.0.0.1:9090/servers/deleteServer?id=<ID>`
Deletes a  "server" object matching with ID.

## RestController interface extends MongoRepository

```java
List<Server> findAll();
    
Optional<Server> findById(String Id);
    
void createOrUpdateServer(Server server);
    
void deleteServerById(String Id);
    
List<Server> findByName(String name);
```

### Using Postman

Run the following created collection to Test and consume the APIs

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/5ff40fbad3968a1b28b0)

**NOTE:** *The above collection is created and tested for `http://127.0.0.1:9090/servers/` endpoint*

### Screenshots


