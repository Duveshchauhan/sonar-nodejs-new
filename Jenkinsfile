node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def scannerHome = tool 'SonarScanner'; 
    withSonarQubeEnv() {
      sh "${scannerHome}/sonar-scanner"
    }
    
}
}
