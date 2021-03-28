# deploying-docker-on-asw
Deploy docker on aws and try out small applications.


- I created an EC2 instance on aws
- then I connected to this instance with putty
- afterwards installed docker on this instance. Here I made use of the following [aws instructions](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/docker-basics.html)
- installation of docker: `sudo apt install docker` 
- creation of Dockerfile: `touch Dockerfile`
- use nano to edit the content of the Dockerfile in the terminal
- build an image: `docker build -t hello-world .`
- start the container: `docker run -t -i -p 80:80 hello-world`
- try the application in a web browser by using the public IPv4 DNS of the instance
