Vul onderstaande aan met de antwoorden op de vragen uit de readme.md file. Wil je de oplossingen file van opmaak voorzien? Gebruik dan [deze link](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) om informatie te krijgen over
opmaak met Markdown.

a)
### Working with docker in JENKINS

To work with docker in jenkins first install docker on the machine where JENKINS is installed.

![img](./IMAGES/installing_docker.png)

After installing docker you will  notice that it can't be ran by a normal user, only by sudoers.
To fix this we will add our users who  need to use the DOCKER commands to the "docker" group.

To do this follow this guide: 

1. OPEN A TERMINAL
2. EXECUTE THE FOLLOWING COMMANDS:
![img.png](IMAGES/adding_personal_user.png)

![img.png](IMAGES/adding_jenkins_user.png)

The first command will add our personal user to the docker group, of course assuming that the "$USER" enviorment variable
is filled in. To check this type the following command: "echo $USER"

Now let's move over to JENKINS.

### Jenkins and Docker

## Installing the docker plugin

To begin using docker in our scripts we will need to add the docker plugin to our jenkins.

![img.png](IMAGES/docker_plugin.png)

Now that is done we will  need to add a docker credential to  "JENKINS".

You can follow the same steps from our previous excercise to add a credential of your "DOCKER USER NAME" and "DOCKER USER PASSWORD".

![img.png](IMAGES/Adding_docker_credential.png)

Once that's done you can begin using DOCKER in your jenkinsfile.


b)


