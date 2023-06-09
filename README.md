# MySQL-Week7-Assignment

MySQL Java Maven Project
This repository contains the implementation of a Java Maven project using MySQL Workbench to create a schema and user, and to assign schema privileges to a user.

Objectives
In this project, we aim to:

Create a schema and a user using MySQL Workbench.
Assign schema privileges to a user with MySQL Workbench.
Create a Maven project in Eclipse.
Add MySQL driver as a dependency in pom.xml.
Separate project concerns by creating different packages.
Write Java code to connect to a MySQL database and schema.
Setup
Creating a Schema with MySQL Workbench
The project utilizes a schema named 'projects'. A user named 'projects' is also created and assigned a password. This user is granted all privileges, except the "GRANT OPTION".

Maven Project
A Maven project is created with the Group ID com.promineotech, Artifact ID mysql-java, and Version 0.0.1-SNAPSHOT.

Pom.xml Modifications
The MySQL driver is added as a dependency in pom.xml, and the Maven compiler plugin is configured according to the instructions detailed in this project.

Project Packages
The project structure includes the following packages and subpackages under src/main/java:

projects
projects.dao
projects.entity
projects.exception
projects.service
Exception Class
The DbException class is created in the projects.exception package and extends RuntimeException.

JDBC Connection Class
A class named DbConnection in the projects.dao package is created to obtain a JDBC Connection object from the driver manager.

Main Class
An entry point for the application is established with a main() method in the ProjectsApp class in the projects package.

Git Configuration
To ensure that only source code is pushed to this GitHub repository, a .gitignore file is added to the project root directory with the following entries:

Copy code
.settings/
target/
These settings ensure that built class files and additional configuration files maintained by Eclipse are not included in the Git repository.

Solutions
The solutions for the pom.xml, DbConnection.java, ProjectsApp.java, .gitignore, and DbException.java can be found within the respective source code files in this repository.
