## Note: This repo is no longer maintained.  Please visit https://github.com/saucelabs-rdc-sample-frameworks/RDC-Java-TestNG-Appium-Android-REST for up to date code.

## Java-TestNG-Appium-Android-REST

>This code is presented as an example only, since your tests and testing environments may require specialized scripting. This information should be taken only as an
>illustration of how one would set up tests with Sauce Labs, and any modifications will not be supported. For questions regarding Sauce Labs integration, please see 
>our documentation at https://wiki.saucelabs.com/.

### Environment Setup

1. Global Dependencies
    * Install Maven
    	https://maven.apache.org/install.html
    * Or Install Maven with Homebrew
    	http://brew.sh/
    ```
    $ brew install maven
    ```
2. TestObject Credentials
    * Add your TestObject API Key and Appium Endpoint you would like to run against
    ```
    $ export TESTOBJECT_API_KEY=<your project's api key>
    $ export APPIUM_URL=<your preferred appium endpoint URL>
    ```

3. Project Dependencies
    * Check that packages are available
    ```
    $ cd Java-TestNG-Appium-Android-REST
    $ mvn test-compile
    ```
    * You may also want to run the command below to check for outdated dependencies. Please be sure to verify and review updates before editing your pom.xml file as they may not be compatible with your code.
    ```
    $ mvn versions:display-dependency-updates
    ```
4. Application
    * Application can be downloaded by clicking [here](https://github.com/testobject/calculator-test-gradle/blob/master/Calculator_2.0.apk)
    
### Running Tests
	* Note: pom.xml settings and testng.xml need to be updated if you wish to run on more than 2 devices at once.

#####Execute TestNG Suite:
```
$ mvn test -U -Pappium-tests
```

### Advice/Troubleshooting
1. It may be useful to use a Java IDE such as IntelliJ or Eclipse to help troubleshoot potential issues. 

### Resources
##### [TestObject REST API Documentation](https://api.testobject.com/)

##### [Sauce Labs Documentation](https://wiki.saucelabs.com/)

##### [TestNG Documentation](http://testng.org/doc/documentation-main.html)

##### [Java Documentation](https://docs.oracle.com/javase/7/docs/api/)

##### [Stack Overflow](http://stackoverflow.com/)
* A great resource to search for issues not explicitly covered by documentation.







