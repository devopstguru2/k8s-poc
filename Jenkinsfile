pipeline {
    agent any

    stages {
        stage('chekout') {
            steps {
                echo 'Hello World'
            }
        }

        stage("build"){
            steps{
                echo "Building image"
            }
        }
        stage ("Deploy"){
            steps{
                echo "In Deploy block"
            }
        }
        stage("Notify"){
            steps{
                step{
                    
                    echo "Notify to slack channel"
                }
            }
        }
    }
}

