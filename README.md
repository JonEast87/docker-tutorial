# Docker Tutorial

**Following along with Patrick Loeber's [Patrick](https://www.youtube.com/watch?v=0H2miBK_gAk) tutorial on how to dockerize apps**

## Requirements

1. FastAPI
2. UVICORN

### Command to build image
> docker build -t fastapi-image .

### Command to run
**This command runs the docker image and detaches it from the terminal so other commands can be ran in parallel**
> docker run --name fastapi-container -p 80:80 -d fastapi-image

### Command to stop and clear
**Stops the current instance**
> docker stop fastapi-container

**To remove the container**
> docker rm fastapi-container