I created dinorows/georgemichael5000 by running docker build . -t dinorows/georgemichael5000 on my local DockerToolbox on a git shell

Successfully tagged dinorows/georgemichael5000:latest
SECURITY WARNING: You are building a Docker image from Windows against a non-Windows Docker host. All files and directories added to build context will have '-rwxr-xr-x' permissions. It is recommended to double check and reset permissions for sensitive files and directories.

winpty docker login
docker push dinorows/georgemichael5000

FOr some reason, did not work and had to rebuild from AWS Liux AMI (Centos)

test:
docker run -d -p 8080:5000 --name webapp dinorows/georgemichael5000