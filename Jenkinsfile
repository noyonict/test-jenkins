pipeline {
    agent any
    
    environment {
        NEW_VERSION = '1.2.0'
    }

    stages {

        stage("build"){
            steps {
                echo "Change made by ${CHANGE_AUTHOR} for the ${CHANGE_BRANCH}"
                echo "This build is builded by ${NODE_NAME}-${NODE_LABELS}-${GIT_AUTHOR_NAME}"
                echo "Build stage"
                echo "Build stage for auto trigger"
                echo "Testing Environment variable ${NEW_VERSION}"
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
