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
                sh 'python3 --version'
            }
        }
        
        stage("regression testing") {
            parallel {
                stage('chrome') {
                    steps {
                        echo 'Chrome'
                    }
                }
                stage('firefox') {
                    steps {
                        echo 'Firefox'
                    }
                }
                stage('safari') {
                    steps {
                        echo 'Safari'
                    }
                }
            }
        }

        stage('release'){
            steps {
                echo 'Release'
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
