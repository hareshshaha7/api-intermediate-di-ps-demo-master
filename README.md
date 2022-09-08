# api-intermediate-di-ps-demo
Added Burger API For Demo
Added Newman collection json file to run in Jenkins Pipeline
Added burger_v1.yaml file

Added Test CI/CD Pipeline - Test


# To run the Burger App and test with newman
# Move to Burger directory
cd burger

# Package the app
mvn package

# Run the app
java -jar target/burger-0.0.1-SNAPSHOT.jar

# Install Newman
npm install -g newman

# Run tests with Newman
newman run BurgerAPI.postman_collection.json