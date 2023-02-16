
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               sh 'g++ intro.cpp -o intro'
               echo "This is my first step"
            }
        }
        
    
        stage('Test') {
            steps{
            sh 'echo "This is my Test step"'
            }
        }
        stage('Deploy') {
            steps {
              sh 'echo "This is my Deploy step"'
            }
        }
    }
    
    
}

