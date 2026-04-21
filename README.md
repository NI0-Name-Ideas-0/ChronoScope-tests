# Test Guide For Frontend E2E Tests
To end-to-end test the frontend, git pull the current backend repository and run it with the following command:
```
./mvnw spring-boot:run -Dspring-boot.run.arguments="--spring.profiles.active=dev"
```
This hosts the application on localhost:8080 and sets the security configuration to allow requests from localhost:4200, 
which is where the frontend will be hosted after running `ng serve` in the frontend repository.
Angular is configured to set localhost:8080 as the backend url when ran locally.
