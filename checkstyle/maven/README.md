# Maven checkstyle plugin
Add plugins in pom.xml

```xml
<build>
	<plugins>
		<plugin>
			<groupId>org.apache.maven.plugins</groupId>
			<artifactId>maven-checkstyle-plugin</artifactId>
			<version>3.0.0</version>
			<configuration>
				<encoding>UTF-8</encoding>
				<consoleOutput>true</consoleOutput>
				<failsOnError>true</failsOnError>
				<linkXRef>false</linkXRef>
				<configLocation>google_checks.xml</configLocation>
			</configuration>
			<executions>
				<execution>
					<goals>
						<goal>check</goal>
					</goals>
				</execution>
			</executions>
		</plugin>
	</plugins>
</build>
```