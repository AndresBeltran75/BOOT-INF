<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>2.7.3</version>
		<relativePath/> <!-- lookup parent from repository -->
	</parent>
	<groupId>com.transunion</groupId>
	<artifactId>dependencias</artifactId>
	<version>1.1</version>
	<name>dependencias</name>
	<description>prueba de dependencias</description>
	<properties>
		<java.version>1.8</java.version>
	</properties>
	<dependencies>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
		</dependency>
	</dependencies>

	<build>
		<plugins>
	      <plugin>
	        <artifactId>maven-assembly-plugin</artifactId>
	        <configuration>
	          <descriptorRefs>
	            <descriptorRef>jar-with-dependencies</descriptorRef>
	          </descriptorRefs>
	        </configuration>
	        <executions>
	          <execution>
	            <id>make-assembly</id> <!-- this is used for inheritance merges -->
	            <phase>package</phase> <!-- bind to the packaging phase -->
	            <goals>
	              <goal>single</goal>
	            </goals>
	          </execution>
	        </executions>
	      </plugin>
		</plugins>
	</build>

</project>
