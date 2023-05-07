pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-jenkins-christineoeo -Dsonar.organization=devsecops-jenkins-christineoeo -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b613595470b47c1adfcd2e6dd185402b32db3a5e'
			}
        } 
  }
}
