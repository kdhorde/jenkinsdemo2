node {
   try{ 
    stage('checkout code'){
        checkout scm
    }
    stage('Extract data'){
        bat 'C:\\Users\\HP\\AppData\\Local\\Programs\\Python\\Python313\\python.exe extract_data.py'
    }
 }
 catch(err){
    echo "pipeline error: ${err}"
 }
 finally {
    echo "pipeline completed"
 }
}

























// pipeline {
//  agent any
//  environment {
//    python = "C:\\Users\\HP\\AppData\\Local\\Programs\\Python\\Python313\\python.exe"
//  }
//  stages {
//     stage('checkout code'){
//        steps{
//          checkout scm
//        }
//     }
//     stage('Extract data'){
//         steps{
//           bat "${env.python} extract_data.py"
//         }
//     }
//  }
//  post {
//     success {
//      echo "success.."
//     }
//     failure {
//     echo "failure..."
//     }
//     always {
//     echo "always..."
//     }
//  }

// }