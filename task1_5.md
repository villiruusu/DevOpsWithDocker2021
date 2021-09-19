1. `docker pull devopsdockeruh/simple-web-service:alpine`
2. `docker images`

| REPOSITORY        | TAG           | SIZE  |
| :------------- |:-------------| :-----|
| devopsdockeruh/simple-web-service      | ubuntu | 83MB |
| devopsdockeruh/simple-web-service      | alpine      |   15.7MB |

3. `docker run -d -it --name alpine  devopsdockeruh/simple-web-service:alpine`
4. Open new terminal
5. `docker exec -it alpine`
6. `tail -f ./text.log`
7. `Secret message is: 'You can find the source code here: https://github.com/docker-hy'`
8. `docker kill alpine; docker rm alpine;`

