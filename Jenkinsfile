
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
    try {
        sh 'echo "might fail"'
    }
    catch (err) {
        echo "Caught: ${err}"
        currentBuild.result = 'FAILURE'
    }
    
    
}

