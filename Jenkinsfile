pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=hi3ndtran -Dsonar.organization=hi3ndtran -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9ea4f3342cf78ba31f80048b6068cb84c5d2a9db'
			}
        } 
  }
}
