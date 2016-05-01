# Docker, Jenkins, SonarQube


## Prerequire

To use this program, you must have `docker` and `docker-compose` installed on your computer. The installation process can be found on the [official Docker website](https://www.docker.com/)

## Start! 

First of all, you have to clone the project in your directory with the following command:
```Bash
git clone https://github.com/galexandre/docker-jenkins-sonarqube.git
```

Then, go to the `jenkins` directory and execute the following commands. The commands will give the right to the container to execute the files.

```Bash 
chmod 777 jenkins.sh
chmod 777 plugins.sh
chmod 777 init.groovy
```

Now, you can start the program via the following command:

```Bash
docker-compose up
```

## License

This repository is under the MIT license. You can find it [here](https://github.com/galexandre/docker-jenkins-sonarqube/blob/master/LICENSE).
