Create Spring Boot Project using h2 database
Create Product Management Project (using microservices) (Don't create registry and api)
Create 2 Microservices.
1.Product - (id, type), All fields are mandatory (type should be mobile, laptop)
Create API
Get Prodcut By ld;
Get Products By type;
Get ProductsAndDesc by id;
Post new Product
2. ProductDescription (id,brand,model, prize ) All fields are mandatory
Create API
Get byid;
Post new ProductDescription

Test them and keep in your system.
Do it in your VM provided by IIHT.
Do maven clean and zip the file.
Push this 2 microservices on github and send the
Zip files and links to github only; ( No jars should be uploaded )


Create a docker image of microservice I and 2;
Push them on docker hub.
Pull them on AWS EC2 instance
Test it from your Rest Client( VS Code Thunder Client or Postman)




student-service-0.0.1-SNAPSHOT.jar
docker pull madupu/alu-student-service
 

<dependency>
	<groupId>org.springdoc<groupId> 
	<artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
	<version>2.5.0</version>  
</dependency>


 
 <plugin>
				<groupId>org.sonarsource.scanner.maven</groupId>
				<artifactId>sonar-maven-plugin</artifactId>
				<version>3.11.0.3922</version>
			</plugin>
			<plugin>
				<groupId>org.jacoco</groupId>
				<artifactId>jacoco-maven-plugin</artifactId>
				<version>0.8.12</version>
				<executions>
					<execution>
						<id>prepare-agent</id>
						<goals>
							<goal>prepare-agent</goal>
						</goals>
					</execution>
					<execution>
						<id>report</id>
						<goals>
							<goal>report</goal>
						</goals>
					</execution>
				</executions>
			</plugin>









   clean org.jacoco:jacoco-maven-plugin:prepare-agent install
sonar:sonar -Dsonar.login=sqa_49bca2fca1deb861c1210799e63b5f3c306984f3 
