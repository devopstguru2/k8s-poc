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
                def userIdsString = userIds.collect { "<@$it>" }.join(' ')
                slackSend(color: "good", message: "$userIdsString Message from Jenkins Pipeline")
                echo "Notify to slack channel"
            }
        }
    }
}

