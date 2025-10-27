pipeline {
 agent any
 environment {
   python = "C:\\Users\\HP\\AppData\\Local\\Programs\\Python\\Python313\\python.exe"
 }
 stages {
    stage('checkout code'){
       steps{
         checkout scm
       }
    }
    stage('Extract data'){
        steps{
          bat "${env.python} extract_data.py"
        }
    }
 }
 post {
    success {
     echo "success.."
    }
    failure {
    echo "failure..."
    }
    always {
    echo "always..."
    }
 }

}