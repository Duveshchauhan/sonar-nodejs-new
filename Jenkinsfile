node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def scannerHome = tool 'SonarQubeScanner'; 
    withSonarQubeEnv() {
      sh "${scannerHome}/sonar-scanner"
    }
    withSonarQubeEnv('SonarQube') {
  // sh "ls ${scannerHome}"
  // sh "echo ${scannerHome}"
     
      // sh "pwd"
      // sh "/opt/sonar-scanner/bin/sonar-scanner -Dproject.settings=sonar-project.properties"
               
    }
}
  }
}
