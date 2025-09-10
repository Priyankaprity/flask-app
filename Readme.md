#step:1 Open your temninal and navigate to your proj directory
##method 1:
Open your Ubuntu terminal (via Start Menu or wsl command).
Navigate to your project folder using the correct WSL path (cd /mnt/d/Projects/Flask).

##method 2:
Build your Docker image using the docker build command.

#step2:
Start a new container from your image with the docker run command.
docker build -t flask-image .

#step3:
run the img to create container : docker run -d -p5000:5000 --name flaskcontainer flask-image
Confirm the container is running with docker ps.

#step4:
Access the application by opening a web browser and navigating to http://localhost:5000.
