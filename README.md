# ConfigServerFlightsApi
## A Spring Cloud Config Server to fetch configuration for flights-api from github as backend. It needs to run to support the flights-api for fetching profile specific configurations

A Spring Boot app, which serves as a Config Server. It points to https://github.com/AmmadHassanPro/flights-api-configuration github repo to get flights-api.yml , which has Spring profile specific configurations. 

## Running Instructions
Download the code, and on the root of the project, type  ./gradlew bootRun
The config server will be available at http://localhost:8888

### Configuration 
- To point it to another github repo change the property spring.cloud.config.server.git.uri in application.properties file.
- To change the port, change the property at server.port in application.properties.
### flights-api repo
https://github.com/AmmadHassanPro/flights-api
