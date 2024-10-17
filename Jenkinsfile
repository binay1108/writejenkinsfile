
pipeline {
    agent any
    stages{
        stage("build") {
            steps {
                echo 'building the application'
            }
        }
        
        stage("test") {
            steps {
                echo 'testing the application'
            }
        }
        
        stage("deploy") {
            steps {
                echo 'deploying the application'
            }
        }
    }
    post {
        always {
            echo 'Always run this no matter if pipeline is successful or failed'
            echo 'Build Status is ----'
        }
        success {
            echo 'The buld has been successful'
        }
        failure {
            echo ' The build has failed'
        }
    }
}
