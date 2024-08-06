@Library('my-shared-library') _

pipeline{
    

    agent any

    stages{

        stage(' Git Checkout'){

            steps{
                script{

             gitCheckout{
                    url : "https://github.com/panduvallabhasetti/javanew.git"
                    }
                }
            }
        }
    } 


}
