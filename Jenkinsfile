node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def scannerHome = tool 'SonarQubeScanner';
    // withSonarQubeEnv() {
      // sh "${scannerHome}/bin/sonar-scanner"
    // }
    withSonarQubeEnv() {
  sh "ls ${scannerHome}"
  sh "echo ${scannerHome}"
}
  }
}
