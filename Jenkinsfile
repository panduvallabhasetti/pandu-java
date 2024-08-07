@Library('my-shared-library') _
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                gitCheckout(
                    url : 'https://github.com/panduvallabhasetti/pandu-java.git'
                    )
                }
            }
        }
    }
}
