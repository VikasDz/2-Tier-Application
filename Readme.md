DockerHub (Login in DockerHub)
Change Your Docker Image Name With DockerHUBImageName
{
    1.(docker tag flask-api:latest vikashkumar97/microservices-flask-api:latest)
    2.docker images (Name Changed)
    3.docker push vikashkumar97/microservices-flask-api:latest(Push Your Docker Image)
    4.docker run -d -p 5000:5000 vikashkumar97/microservices-flask-api:latest

}
Docker Compose Make Network Also Between Two Docker Containers
DockerCompose {

    docker ps
    YAML File (dockerCompose.yaml)
    Simple JSON

    version : "3.9"
    services :
        flask-api:
            image: vikashkumar97/microservices-flask-api:latest
            container_name: microservices-flask-api
        ports:
           -"5000:5000"
        mongo-db:
            image: mongo
            container_name: mongo
            ports:
                - "27017:27017"
        

    (sudo install docker-compose)
    docker-compose up -d (Create)
    docker-compose down (Kill or Down Container)


}
Project - Microservices , Database CURD Applications
Docker Network (Host , Bridge ,Overlay Network)
Docker Swarm
Monolith : - Single Application
Microservices : - Lots of Services Ruuning on Services ..
Like : facebook.com/auth , Facebook.com/singup
API
Using Postman [GET, POST, PUT, DELETE, PATCH]
Volume : Volume is a place where you can Store Containers Data


Docker Hub is a cloud-based registry service that allows you to store and manage Docker images. It provides a centralized platform for sharing, distributing, and collaborating on containerized applications. Docker Hub facilitates the discovery and distribution of Docker images, making it a key resource in the Docker ecosystem.

Docker Compose is a tool for defining and running multi-container Docker applications. It allows you to describe your application's services, networks, and volumes in a docker-compose.yml file, and then use a single command to start and run your entire application stack.

