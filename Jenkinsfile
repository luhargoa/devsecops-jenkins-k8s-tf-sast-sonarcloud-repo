pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Devsecops-Udemy -Dsonar.organization=Devsecops-Udemy -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=4e388f04471c5755d9250b92f16ad843a3e89c01'
			}
        } 
  }
}
