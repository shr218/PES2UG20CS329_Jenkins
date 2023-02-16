
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
                sh './intro'
                echo "This is my Test step"
            }
        }
        stage('Deploy') {
            steps {
              sh 'echo "This is my Deploy step"'
            }
        }
    }
    post{
        failure {
                echo 'only when the Pipeline is currently in a "failed" state run, usually expressed in the Web UI with the red indicator.'
        }
    }
    
    
    
}

