# theia-docker-basic
Basic template for the Theia IDE running with Docker

# Building

docker build -t tag/here .

or with proxy 

docker build --build-arg proxy="http://host:port" -t tag/here .


# Running

docker run -it --init -p 3000:3000 -v "$(pwd):/home/project:cached" tag/here