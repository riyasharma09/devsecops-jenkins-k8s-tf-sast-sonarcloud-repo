pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:4.0.0.4121:sonar -Dsonar.projectKey=buggywebapp09 -Dsonar.organization=BuggyWebApp09 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=be3ddb64c647283583b81b8709f2f89f5bfa05ed'
			}
        } 
  }
}
