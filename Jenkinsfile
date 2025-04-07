pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vincebuggywebapp -Dsonar.organization=VinceBuggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b5755d9ec708a6388ee8bde630dba1e2245a2393'
			}
        } 
  }
}
