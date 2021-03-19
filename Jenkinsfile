pipeline{
  agent any
                 
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
      sh "bsh deploy-script.sh"}
    }
  }
