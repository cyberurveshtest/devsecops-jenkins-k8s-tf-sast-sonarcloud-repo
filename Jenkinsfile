pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dipanshujenkins -Dsonar.organization=dipanshujenkins -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5db07802240f7082c5211803c50a1b43b923a48e'
			}
        } 
  }
}
