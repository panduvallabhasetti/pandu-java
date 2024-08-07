@Library('my-shared-library') _
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                gitCheckout(
                    branch : 'master',
                    url : 'https://github.com/panduvallabhasetti/pandu-java.git'
                )
            }
        }
        stage('mvn Unit Test'){
             steps {
                script{
                    mvnTest()
                }
             }
        }
    }
}
