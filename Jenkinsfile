@Library('my-shared-library') _
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                gitCheckout{
                    url : 'git 'https://github.com/panduvallabhasetti/pandu-java.git'
                }
            }
        }
    }
}
