pipeline {
    agent any

    stages {

        stage("build"){
            steps {
                echo "Build stage"
                echo "Build stage for auto trigger"
            }
        }

        stage("test"){
            steps {
                echo "test stage for auto trigger"
            }
        }

        stage("deploy"){
            steps {
                echo "deploy stage for auto trigger"
            }
        }
    }
    post {
        always {
            echo "Run Always"
        }
        success {
            echo "Run success"
        }
        failure {
            echo "Run failure"
        }
    }
}
