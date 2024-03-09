# Sonarqube Local Project
Static Testing  - SonarQube local code analysis



## Setting environment
### Requeriments:

#### Java JDK Version
      * Java 11 or 17 (prefered 17 version )
      
      * JAVA_HOME environment

#### Sonarqube 
      Download sonarqube (free version):
      ->  https://www.sonarsource.com/products/sonarqube/downloads/

#### Sonar Scanner
     *  Download sonar Scanner
      -> https://docs.sonarsource.com/sonarqube/latest/analyzing-source-code/scanners/sonarscanner/


     * setting sonnarscanner to global env
     -> sonar-scanner --version


#### Running Sonarqube 

     * Run startSonar.bat from sonarqube dir:
       ./bin/win64/StarSonar.bat

     * Open localhost:9000 

     * Log in to web ( user: admin | pass: admin )
       -> change password



#### SonarScanner properties:
     -> edit sonnar-scanner configs (sonar-scanner.properties)
          sonar.projectKey=wdio-1
          sonar.projectName=wdio-1
          sonar.projectVersion=1.0
          sonar.sources=C:/Users/Jean/Desktop/files/code/QA/Automation/WebdriverIO/wdio-1/test
          sonar.exclusions=
          sonar.languages=ts


#### Getting User Token:
      -> Go to profile and get User token 
      e.g. : 
        token =  squ_2728df22208b73bd938338e6963bbcd7256075ba


#### Scanning project: 
     * Open CMD in specific project dir


     * execute command:
        TOKEN= squ_2728df22208b73bd938338e6963bbcd7256075ba
        sonar-scanner -Dsonar.login=${{TOKEN}}






