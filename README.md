# Docker, Jenkins, SonarQube

## 1. Docker

To use this program, you must have `docker` and `docker-compose` installed on your computer. The installation process can be found on the [official Docker website](https://www.docker.com/)

## 2. Start the program

First of all, you have to clone this project in your directory with the following command:
```Bash
git clone https://github.com/galexandre/docker-jenkins-sonarqube.git
```

Then, go to the `jenkins` directory. Execute the following command. 

```Bash 
chmod 777 jenkins.sh
```

The command will give the right to the container to execute the file `jenkins.sh`.

Now, you can start the program via the following command:

```Bash
docker-compose up
```

## 3. Jenkins and SonarQube

Jenkins and SonarQube are available on the following ports:

- Jenkins: 8080
- SonarQube: 9000

At the first start, Jenkins will ask you for a password. This password is displayed in the log. However, you can have access to this password via the container. 

To create a connection to the container, you have just to do this command:
```Bash 
docker exec -i -t jenkins bash
```
Use the command cat on the specific file and copy the password.

## 4. Connection between Jenkins and SonarQube

//TODO

## License

This repository is under the MIT license. You can find it [here](https://github.com/galexandre/docker-jenkins-sonarqube/blob/master/LICENSE).
