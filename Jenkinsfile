pipeline{
    @library('my-shared-library') _

    agent any

    stages{

        stage(' Git Checkout'){

            steps{

                script{

                     gitCheckout{
                        branch = "main"
                        url = "https://github.com/panduvallabhasetti/javanew.git"
                     }
                }
            }
        }
    } 


}