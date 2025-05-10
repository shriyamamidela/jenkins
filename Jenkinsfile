pipeline {
    agent { 
        node {
            label 'docker-agent'
        }
    }
    triggers {
        pollSCM '*/5 * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                echo "Building from Jenkins file"
                echo "By Shriya Mamidela-SE22UCSE250"
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                echo "Testing the build triggered from Jenkins file."
                echo "By Shriya Mamidela-SE22UCSE250"
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                echo "By Shriya Mamidela-SE22UCSE250"
                '''
            }
        }
    }
}
