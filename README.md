### Spring Boot Eureka Demo

#### Eureka Server

Start the server

```
cd eureka-server
mvn spring-boot:run
```

Visit the Eureka dashboard at http://localhost:8761

Note that there are no 'Instances' yet registered


#### Eureka Client

Start up a client

```
cd eureka-client
mvn spring-boot:run
```

Visit the client directly at http://localhost:8080/

You can also visit the Eureka dashoboard again now and see it listed there.


#### Spin up another client with a different name

You can see that another client will be registred by doing the following:

```
cd eureka-client
mvn spring-boot:run -Dspring.application.name=Second-Instance -Dserver.port=8081