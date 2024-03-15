node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    
      sh "sonar-scanner"
  }
}
