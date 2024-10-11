# Data-Driven-Approach
Data-Driven Framework in Java Selenium
Overview:
This project demonstrates a data-driven testing framework using Java and Selenium. The framework reads test data from an Excel file, allowing easy scalability and maintenance of test cases.

Features:
Excel Data Integration: Utilizes Apache POI to read and write Excel files for test data.
Selenium WebDriver: Automates web browser actions.
Modular Design: Easily extendable for different test scenarios.
Cross-Browser Testing: Configurable to run on multiple browsers.

Prerequisites:
Java Development Kit (JDK)
Apache POI library
Selenium WebDriver
ChromeDriver (for Chrome browser testing)

Installation:
Clone the repository: https://github.com/MrVamc/Data-Driven-Approach.git

Add dependencies: Add the following dependencies to your pom.xml if you're using Maven:

<artifactId>DataDrivenFramework</artifactId>
	<version>0.0.1-SNAPSHOT</version>



	<properties>
		<maven.compiler.target>11</maven.compiler.target>
		<maven.compiler.source>11</maven.compiler.source>


	</properties>


	<dependencies>
		
		

		<!-- https://mvnrepository.com/artifact/org.testng/testng -->
		<dependency>
			<groupId>org.testng</groupId>
			<artifactId>testng</artifactId>
			<version>6.14.3</version>
		</dependency>


			<!--
		https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-java -->
		<dependency>
			<groupId>org.seleniumhq.selenium</groupId>
			<artifactId>selenium-java</artifactId>
			<version>4.16.1</version>
		</dependency>


		<!-- https://mvnrepository.com/artifact/com.aventstack/extentreports -->
		<dependency>
			<groupId>com.aventstack</groupId>
			<artifactId>extentreports</artifactId>
			<version>5.1.1</version>
		</dependency>



		<!-- https://mvnrepository.com/artifact/log4j/log4j -->
		<dependency>
			<groupId>log4j</groupId>
			<artifactId>log4j</artifactId>
			<version>1.2.17</version>
		</dependency>

		<!-- https://mvnrepository.com/artifact/com.sun.mail/javax.mail -->
		<dependency>
			<groupId>com.sun.mail</groupId>
			<artifactId>javax.mail</artifactId>
			<version>1.6.2</version>
		</dependency>

		<!-- https://mvnrepository.com/artifact/commons-io/commons-io -->
		<dependency>
			<groupId>commons-io</groupId>
			<artifactId>commons-io</artifactId>
			<version>2.15.1</version>
		</dependency>


		<!-- https://mvnrepository.com/artifact/mysql/mysql-connector-java -->
		<dependency>
			<groupId>mysql</groupId>
			<artifactId>mysql-connector-java</artifactId>
			<version>6.0.5</version>
		</dependency>


		<!-- Dependency for POI API -->
		<!-- http://mvnrepository.com/artifact/org.apache.poi/poi -->
		<dependency>
			<groupId>org.apache.poi</groupId>
			<artifactId>poi</artifactId>
			<version>3.6</version>
		</dependency>

		<!-- http://mvnrepository.com/artifact/org.apache.poi/poi-ooxml -->
		<dependency>
			<groupId>org.apache.poi</groupId>
			<artifactId>poi-ooxml</artifactId>
			<version>3.6</version>
		</dependency>
		<!-- http://mvnrepository.com/artifact/dom4j/dom4j -->
		<dependency>
			<groupId>dom4j</groupId>
			<artifactId>dom4j</artifactId>
			<version>1.1</version>
		</dependency>

		<!-- http://mvnrepository.com/artifact/org.apache.xmlbeans/xmlbeans -->
		<dependency>
			<groupId>org.apache.xmlbeans</groupId>
			<artifactId>xmlbeans</artifactId>
			<version>2.3.0</version>
		</dependency>

		<!-- http://mvnrepository.com/artifact/org.apache.poi/poi-ooxml-schemas -->
		<dependency>
			<groupId>org.apache.poi</groupId>
			<artifactId>poi-ooxml-schemas</artifactId>
			<version>3.6</version>
		</dependency>


	</dependencies>


	<build>
		<plugins>

			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-surefire-plugin</artifactId>
				<version>2.18.1</version>
				<configuration>
					<testFailureIgnore> false </testFailureIgnore>
					<suiteXmlFiles>
						<suiteXmlFile>src/test/resources/runner/testng.xml</suiteXmlFile>

					</suiteXmlFiles>
				</configuration>


			</plugin>


		</plugins>

Contributing:
Feel free to fork this project and make contributions. Pull requests are welcome!
