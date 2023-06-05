#####build in order to create image in docker, (--tag tictac:0.0.2 is version)
docker build ./ --tag tictac:0.0.2 
###run image in order to create container (post run on browser 8000, app post: 5173)
docker run -dit -p 8000:5173 --name tictac4 tictac:0.0.2
#remove contaniner unuse
docker container prune
docker run -dit --name ubuntu_1 ubuntu:20.04
docker run -dit -p 3000:5173 --name tictac1 tictac:0.1
docker ps

