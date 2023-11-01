pipeline {
    
    agent any

    stages {
        stage("build"){
            steps {
                python3 -v
            }
        }
    }

    post {

        always {
            echo "It's a learning process!"
        }

        success {
            echo "Success"
        }

        failure {
            echo ' Failed'
        }

        unstable {
            echo "Unstable"
        }

        changed {
            echo 'Changed'
        }
    }
}
