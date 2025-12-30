//SCRIPTED

//DECLARATIVE
pipeline {
    // agent any
    agent {docker {image 'maven:4.0.0-rc-5-amazoncorretto-25-debian-trixie'} }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
                echo "Build"
            }
        }
        stage('Test') {
            steps {
                echo "Test"
            }
        }
        stage('Integration Test') {
            steps {
                echo "Integration Test"
            }
        }
    }

    post {
        always {
            echo 'Im awesome, I run always'
        }
        success {
            echo 'I run when you are successful'
        }
        failure {
            echo 'I run when you fail'
        }
    }
}
