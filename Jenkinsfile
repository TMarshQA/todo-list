pipeline{
  agent any
  environment {
    DATABASE_URI = credentials ("DATABASE_URI")
    SECRET_KEY = credentials ("SECRET_KEY")
                 
  stages{
    stage('Install Dependencies'){
      steps{
        sh "bash install-dependencies.sh"
      }
    }
    stage('Test'){
      steps{
        sh "bash test-script.sh"
      }
    }
    stage('Deploy'){
      steps{
      sh "bash deploy-script.sh"}
    }
  }
}
