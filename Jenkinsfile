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
        stage('mvn Integratin Test'){
             steps {
                script{
                    mvnIntegrationTest()
                }
             }
        }
        stage('Static Code Analysis : Sonarqube'){
             steps {
                script{
                    withCredentials([string(credentialsId: 'squ_64b99cb9d3de40e6085d682d9c2691cc417fcfc2', variable: 'SONAR_TOKEN')]) {
                    sh 'mvn sonar:sonar -Dsonar.login=$SONAR_TOKEN'
                    statiCodeAnalysis()
                }
             }
        }
    }
}
