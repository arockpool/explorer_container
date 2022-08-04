# explorer_container

# python
docker build -f Dockerfile_python_base -t explorer_python_base:dev .
# go
docker build -f Dockerfile_go_base -t explorer_go_base:dev .



cp ./docker-compose.yml ./docker-compose-back.yml

#  Remove unused docker commands

# docker create network
docker network create dev_network

# docker compose
docker-compose -f docker-compose.yml up -d

