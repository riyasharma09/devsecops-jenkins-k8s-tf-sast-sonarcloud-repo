pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp09 -Dsonar.organization=BuggyWebApp09
 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=be3ddb64c647283583b81b8709f2f89f5bfa05ed'
			}
        } 
  }
}
