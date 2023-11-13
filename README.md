# DevOps project on Google Cloud

This repository is for the DevOps project deployed on Google Cloud. <br>
We are using the sprint agile methodology for this project and there will be 7 sprints. 

## Technologies
- Python
- Docker
- Google Kubernetes Engine 

### Sprint 1 
#### Write a python application + Dockerfile. Build and run the docker image locally.
- Write a simple python code for "Hello World" <br>
The code(`app.py`) uses a python library called `flask`. We need to download `flask` library in order to run the code. We will simply add `flask` inside `requirements.txt` so that it can be referenced during `docker build`

- Create a Dockerfile <br>
We will use `python:3.8-slim-buster` base image. You can use an image of your choice which has the same version. We will copy the previous `requirements.txt` into our Dockerfile working directory, and install it with `pip3 install`. 

- Build and run the image locally <br>
If you do not have local Docker Desktop setup, please proceed the steps in this <a href="https://docs.docker.com/desktop/install/windows-install/">documentation</a>. <br>
Run the following commands to build and run docker image locally. <br>
    - `docker build -t hello-world .` 
    - Check your image - `docker images`
    - Run the built image - `docker run -p 5001:5000 hello-world` 
    - Access the application on browser via `localhost:5001` 



