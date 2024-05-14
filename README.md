student-service-0.0.1-SNAPSHOT.jar
docker pull madupu/alu-student-service
 
 
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
