pipeline{
 agent any
 stages{
  stage('Checkout') {
    steps {
            git branch: 'main',url: 'https://gitlab.com/Ria-30/pipelines-javascript.git'
          }
  }
  stage('Build'){
    steps {
      sh 'npm i'
    }
  }
  stage('Deploy'){
    steps {
      sh 'npm start'
    }
  }
  stage('SonarQube Analysis'){
    steps {
      sh '
    }
  }
 }
}
