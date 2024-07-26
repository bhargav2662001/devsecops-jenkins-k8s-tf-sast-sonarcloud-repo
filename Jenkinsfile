pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=springApi -Dsonar.organization=springapi -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6f2d4e994ac223f82b2a5ad210dccaf8969b9b87'
			}
        } 
  }
}
