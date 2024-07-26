pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=springboot1_springboot1 -Dsonar.organization=springboot1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=7feb1efc083e3d0a54663f2d73c09a5cd02f82a3'
			}
        } 
  }
}
