pipeline{
  agent any
  stages{
    stage('Install Dependencies'){
      steps{
        sh "python3 -m venv venv"
        sh "source venv/bin/activate"
      }
    }
    stage('Test'){
      steps{
        sh "pip install -r requirements.txt"
      }
    }
    stage('Deploy'){
      steps{
      sh "pip install pytest pytest-cov"}
    }
