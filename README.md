# Flask_Application_Using_Docker
In this project, a Docker container was used to create an isolated development environment to test a Flask application.

Image uploaded to Docker Hub: https://hub.docker.com/r/rokoko24/flask-docker/tags

Steps taken to create, run, and open Docker container using the command line:
  1. Wrote a generic Python program, which included Flask, an html file, requirements.txt file, and Dockerfile
  3. Then the docker image was built on the command line using the docker build command
  4. Then the docker image was run inside of the container using the docker run command
  5. To check the status of any containers Docker Desktop was downloaded (although this can also be done using the docker ps command)
  6. Once you have your container running on a specific port, you can enter the container by using the docker exec command
  7. Then once inside the container, you can run the Python program by typing python followed by the name of your program
  8. This will provide a localhost url that you can enter into a browser in order view your Flask application's output
  
  Tips:
  1. Even if you stop the container, as long as you start the container up again all of your changes that you made inside the container will be saved. If you permanently delete the container, your changes will be lost
  2. You can open multiple containers of the same program to test in, as long as you use different ports
  3. It is easier to use the Docker Desktop application to view which containers are running, but you can also use the docker ps command to view this on the terminal
  4. This whole process is pretty much applicable to any image on DockerHub since we are now using terminal to create, run, and open our containers
  5. You can type localhost:[port number] on the browser to see what the flask application does

Expected Output:
<img width="1440" alt="image" src="https://user-images.githubusercontent.com/81287555/187007804-0b0e82d6-898a-466f-90d6-7aeeaac36ef8.png">
