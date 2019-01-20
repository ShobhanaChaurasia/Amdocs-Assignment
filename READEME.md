Project Name : assignment

Description : 
Create a Maven project to implement a simple Spring based web application with a controller exposing the following 4 APIs
 • GET /user 
 • POST /user 
 • PUT /user 
 • DELETE /user 
 Those APIs will perform CRUD operations using Hibernate as persistence framework on a User entity with at minimum the following fields: 
 • id (long) / primary key 
 • username (String) / unique 
 • password 
 • status (String) / possible values: Activated/Deactivated 
 Secure those 4 APIs with Spring Security using BASIC authentication. 
 Provide unit tests for controllers, services and DAO classes. 
 

 Installation :
1. Eclipse Neon for creating the application.
2. Use Apache Derby DB for perform DB operation.
3. Use Embedded tomcat to run the project.
4. Save the project in the eclipse workspace and imort the project by using the option "Project from existing workspace".
 Make the below configuration to clean , install and run the server
 a. Run As --> Run Configuration --> Maven Build --> (create "maven war build") with below configuration :
	 name - maven war build
	 base directory -  C:/AmdocsSpringProj/assignment
	 goals - clean install
	 click on Run tab.
 b. Run As --> Run Configuration --> Maven Build --> (create "Tomcat Run") with below configuration :
	 name - Tomcat Run
	 base directory - C:/AmdocsSpringProj/assignment
	 goals - tomcat7:run
	 click on the run tab
 
Usage : 
 Install postman and perform the below operation by using the URL "http://localhost:8080/user"
		Save
		Update
		Get
		Delete
		
		Please refer the Artifacts.doc for how to perform the above operation in postman.
		