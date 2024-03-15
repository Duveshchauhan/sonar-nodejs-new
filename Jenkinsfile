node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    
      sh "${scannerHome}/bin/sonar-scanner"
  }
}
