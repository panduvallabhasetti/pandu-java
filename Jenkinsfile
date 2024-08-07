@Library('my-shared-library') _
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                gitCheckout(repo: 'https://github.com/panduvallabhasetti/javanew.git', branch: 'master')
            }
        }
    }
}
