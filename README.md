# Jenkins JDK 11 w/ Maven Docker Image
Custom Docker Image for Jenkins with Maven installed.

## Setting Up
Download the repo as a zip [here](https://github.com/maciejfec2i/dockerised-jenkins-jdk11-with-maven/zipball/main), or fork and pull. <br><br>
Run the following commands:
```
docker build -t jenkins-jdk11-with-maven .

docker run --name jenkins-with-maven -p 8081:8080 -p 50000:50000 -v jenkins-with-maven:/var/jenkins_home jenkins-jdk11-with-maven
```

After that the docerised instance of Jenkins can be started with the Jenkins.bat file, or using the following command:
```
docker start jenkins-with-maven
```