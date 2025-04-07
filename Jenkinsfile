pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vincebuggywebapp -Dsonar.organization=vincebuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=182d66a24de604373489a80b705561d76f4650dc'
			}
        } 
  }
}
