This container runs a Sickbeard server. The container is based on Alpine Linux and ends up being around 65MB in size.

Config
Mount and download or watch directories to the container as a volume to allow access for transferring files.

To build, run, and debug the container use the provided Makefile. 

Ex:

docker pull majormjr/docker-sickbeard
docker run -d -v /sickbeard:/sickbeard -p 8081:8081 majormjr/docker-sickbeard -
