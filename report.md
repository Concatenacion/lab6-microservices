**1. The two microservices are running and registered**

Screenshots of the functioning of the Web Server and Accounts Server services, respectively.

Web Server

![Figure 1](P6/Web_server.png  "Web Server")
![Figure 2](P6/df82a878bc283ab70478bc01e79a800e.png "Web Server Running")

Accounts Server

![Figure 3](P6/Accounts_Server.png "Accounts Server")
![Figure 4](P6/38bcf07de64520dbb5103a1916d2ad8c.png "Accounts server running")


**2. The service registration service has the two microservices registered.**

Screenshots of the Registry service with the two registered services.

![Figure 5](P6/Register_basic.png "Service Registration")
![Figure 6](P6/Registration_server_running.png "Service Registration running")

**3. A second account microservice is running in the port 4444 and it is registered.**

Screenshots of the second Account service.

![Figure 7](P6/Second_account_running.png "Service Registration running")
![Figure 8](P6/Register_4444.png "Server registration with second server accounts.")

**4. A brief report describing what happens when you kill the microservice with port 2222.** 

***Can the web service provide information about the accounts? Why?***

The registration service allows the web service to know that there are two possible accounts services. 
In the event that one of them fails, the web service will ask the registry that another service is available, 
allowing to continue working.
