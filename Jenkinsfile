pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=capozzolo -Dsonar.organization=capozzolo -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=a6169c378e6f166ef355765ea9873fe09e4a2f94'
			}
        } 
  }
}
