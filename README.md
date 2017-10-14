https://spring.io/guides/gs/spring-boot-docker/

BUG:
only works (on http://localhost:80) if you do the following:
1. run '__docker build .__' from root dir
2. docker images to find the IMAGE ID
3. docker run -d -p80:8080 <IMAGE ID>

dockerfile-maven-plugin is failing to build image