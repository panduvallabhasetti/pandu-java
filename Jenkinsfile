@Library('my-shared-library') _
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                gitCheckout{
                    branch : 'master',
                    url : 'git 'https://github.com/panduvallabhasetti/pandu-java.git'''
                }
            }
        }
    }
}
