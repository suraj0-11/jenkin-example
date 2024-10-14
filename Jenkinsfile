pipeline {
  agent { docker { image 'cameronmcnz/ant-jdk8-git:latest' } }
  stages {
    stage('Log Jenkins Maven Docker Git and Java version info') {
      steps {
        echo 'mvn -version'
        echo 'java -version'
	echo 'git --version'
      }
    }
    
    stage('GitHub Jenkins Maven Docker Build') {
      steps {
        echo 'mvn clean compile test install'
      }
    }
  }
}
