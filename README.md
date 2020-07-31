# spring-boot-with-docker

## Docker commands:
Log in to the Docker Hub registry  
`docker login` 
 
Build the Docker image  
`docker build --rm --build-arg JAR_FILE=target/demo-0.0.1-SNAPSHOT.jar -t humbertocsilva/spring-boot-with-docker:latest .`  

Push the image to the Docker Hub registry  
`docker push humbertocsilva/spring-boot-with-docker:latest`  

Run the Docker image  
`docker run -d -it -p 8080:8080 humbertocsilva/spring-boot-with-docker:v1.0`  

## References:  
- https://docs.spring.io/spring-boot/docs/2.3.2.RELEASE/reference/html/spring-boot-features.html#boot-features-container-images
- https://docs.spring.io/spring-boot/docs/2.3.2.RELEASE/maven-plugin/reference/html/#repackage-layers
- https://docs.docker.com/engine/reference/builder/
- https://docs.docker.com/engine/reference/commandline/build/
- https://docs.docker.com/engine/reference/commandline/login/
- https://docs.docker.com/engine/reference/commandline/push/
