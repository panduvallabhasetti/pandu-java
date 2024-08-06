pipeline{
    @library(my-shared-lib) _

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