pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=born2los3built2win -Dsonar.organization=born2los3built2win -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fa11c57ad3b2bc1a57732b5b9a1b949a617572f1'
			}
        } 
  }
}
