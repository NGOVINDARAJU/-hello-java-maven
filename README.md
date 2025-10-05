# Java Maven Build Job in Jenkins

## Objective
Build a simple Java HelloWorld application using Maven in Jenkins.

## Tools Used
- Java JDK 8 or higher  
- Apache Maven  
- Jenkins (LTS)

## Steps

1. Create project structure:
hello-java-maven/
├── pom.xml
└── src/main/java/HelloWorld.java
# Start Jenkins:
- docker run -d -p 8080:8080 jenkins/jenkins:lts
# In Jenkins:
-Go to Manage Jenkins → Tools → Maven → Install automatically
- Create a Freestyle Project
- Add build step: Invoke top-level Maven targets
- Goal: clean package
- Save and Build
# Check Console Output for:
- [INFO] BUILD SUCCESS
