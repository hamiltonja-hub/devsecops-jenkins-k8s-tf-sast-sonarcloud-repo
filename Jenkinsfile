pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=testbuggywebapp -Dsonar.organization=testbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0271f074a0a41107950b662719ebb2bf5ac0da18'
			}
        } 
  }
}
