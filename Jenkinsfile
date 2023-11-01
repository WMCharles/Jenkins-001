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
        
        stage("regression testing"){
            steps {
                parallel {
                    stage('chrome'){
                        steps {
                            echo 'Chrome'
                        }
                    }
                    stage('firefix'){
                        steps {
                            echo 'Firefox'
                        }
                    }
                    stage('safari'){
                        steps {
                            echo 'safari'
                        }
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
