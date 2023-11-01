pipeline {
    
    agent any

    stages {
        stage("build"){
            steps {
                echo 'python3 --version'
            }
        }

        stage("Deployment"){
            steps {
               echo 'python3 -v'
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
