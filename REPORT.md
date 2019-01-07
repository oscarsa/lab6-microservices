# Report - Lab6 - Microservices
## 1. The two microservices are running and registered
Registration service running 
![Registration GUI](images/RegistrationTerminal.png)
![Registration GUI](images/RegistrationGUI.png)

Accounts microservice running
![Registration GUI](images/Accounts1Terminal.png)
![Registration GUI](images/Accounts1GUI2.png)
![Registration GUI](images/Accounts1GUI.png)

Web microservice running
![Registration GUI](images/WebTerminal.png)
![Registration GUI](images/WebGUI.png)
![Registration GUI](images/WebGUI2.png)

Both microservices running
![Registration GUI](images/AccountsAndWeb.png)

## 2. The service registration service has the two microservices registered

![Registration GUI](images/RegistrationAll.png)

## 3. A second account microservice is running in the port 4444 and it is registered

![Registration GUI](images/Accounts2Terminal.png)

![Registration GUI](images/Accounts2GUI.png)

![Registration GUI](images/Accounts2GUI2.png)

## 4. A brief report describing what happens when you kill the microservice with port 2222

![Registration GUI](images/Accounts1Killed.png)

After killing the microservice with port 2222, if a user try to access to the accounts service, there are some seconds when the provided service is unaccessible and it returns a connection refused error.

A few seconds later, when the user try to access again, the Eureka registration service provide the connection details of another active instance of the account service, the port 4444.