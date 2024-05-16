danh tag latest
danh tag va publish to dockerhub
Work with container
    Create container with name
        docker run -d --name your_container_name your_image_name
    Create container with folder

    Start & stop
    publishing port
    watch logs
    Execute commands in container
    Remove containers
    Using volumes store data container
    Share sourc
        docker run -dp 4202:4200 -v //d/Git/docker/angular-app-docker:/app --name angular3 angular
        docker run -dp 4200:4200 --mount type=bind,source="//d/Git/docker/angular-app-docker",target=/app --name angular angular
?? c?u l?nh trong docker file ntn l? h?p l?
Kh?c nhau gi?a c?u l?nh docker run v? docker excec
    docker run: l?nh n?y s? d?ng t?o m?i 1 container v? start
    docker exec: l?nh n?y s? d?ng ?? run command tr?n 1 container ?ang ch?y


