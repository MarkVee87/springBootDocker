https://spring.io/guides/gs/spring-boot-docker/

BUG:
only works (on http://localhost:80) if you do the following:
1. mvn clean install
2. run '__docker build .__' from root dir
3. docker images to find the IMAGE_ID
4. docker run -d -p80:8080 IMAGE_ID

dockerfile-maven-plugin is failing to build image