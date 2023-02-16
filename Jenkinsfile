
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                  echo "This is in build stage"
                  sh 'g++ intro.cpp -o intro'
             
            }
        }
        
    
        stage('Test') {
            steps{
                echo "This is in test stage"
                sh './intro'
                
            }
        }
        stage('Deploy') {
            steps {
              sh 'echo "This is in Deploy stage"'
            }
        }
    }
    post{
        failure {
                echo 'Pipeline Failed'
        }
    }
    
    
    
}

