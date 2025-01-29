# Online Library WebApp Repository

Welcome to the **Kavetec Online Library WebApp** repository! This project is designed to help users appreciate automation by first performing a complete manual deployment workflow before implementing automation with Jenkins.

## 📌 Repository Overview

This repository contains a Java-based web application built with Maven, tested with SonarQube, and deployed on Apache Tomcat. The initial exercise involves manually executing each step of the process to understand the benefits of automation.

## 🚀 Manual Deployment Steps

### Prerequisites
Before proceeding, ensure you have:
- **Java JDK** (at least version 8 or higher)
- **Apache Maven** installed and configured
- **SonarQube** set up for code analysis
- **Apache Tomcat** installed and running
- **Git** installed to clone the repository

### 1️⃣ Clone the Repository
```sh
 git clone https://github.com/Kavetec/online-library-webapp.git
 cd online-library-webapp
```

### 2️⃣ Build the Project with Maven
```sh
mvn clean package
```
This command compiles the source code, runs tests, and packages the application into a WAR file.

### 3️⃣ Analyze the Code with SonarQube
Start SonarQube and then run:
```sh
mvn sonar:sonar
```
Ensure SonarQube is properly configured and running before executing this command.

### 4️⃣ Deploy to Apache Tomcat
Copy the generated WAR file (`target/online-library-webapp.war`) to the Tomcat `webapps/` directory:
```sh
cp target/online-library-webapp.war /path/to/tomcat/webapps/
```
Restart Tomcat to apply changes:
```sh
/path/to/tomcat/bin/shutdown.sh
/path/to/tomcat/bin/startup.sh
```

### 5️⃣ Access the Application
Once deployed, you can access the web application in your browser:
```
http://localhost:8080/online-library-webapp
```

## 🛠 Next Steps: Automating with Jenkins
After successfully completing the manual deployment process, the next step is to automate these tasks using Jenkins. This will help streamline the workflow and eliminate the need for repetitive manual actions.

## 🏆 Learning Outcome
By performing this manual process, you gain an appreciation for the efficiency of automation and the role of CI/CD pipelines in modern software development.


Happy Learning! 🚀

