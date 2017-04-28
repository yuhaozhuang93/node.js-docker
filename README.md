# node.js-docker
Using docker to run node.js
Docker is like a container. You are able to run the images in your container.
Docker can easily build safer apps, ensure tamper-proof transit of all app components and run apps securely on the industry’s most secure container platform. Also, Docker always build for scale, and it is extensible and flexible.

Now, let me introduce some basic instructions.
1. docker ps      (Using to check the running container)
2. docker ps -a   (To see all of the containers)
3. docker images  (To see the images which you have built or download)
4. docker rm  <file name>  (delete the container )
5. docker rmi -f <file name> (delete the image) -f is always required
6. docker build -t <image name> .      (Put all the document in the folder. Open the terminal at the folder)
7. docker run --rm -d -p <port that you want to map>:<port in your Dockerfile> --name <name of your container> <name of image>
   Ex: docker run --rm -d -p 8888:8888 --name myrunningapp mynodeapp
8. docker logs <file name of your container>        Ex: docker logs myrunningapp
