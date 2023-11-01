pipeline {
    
    agent any

    stages {
        stage("build"){
            steps {
                sh 'python3 --version'
            }
        }

        stage("deploy"){
            steps {
               echo 'python3 -v'
            }
        }
        
        // 
        stage('regression testing'){
            steps {
                parallel (
                    chrome: {
                        echo 'Chrome'
                    },
                    firefox: {
                        echo 'Firefox'
                    }
                )
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
