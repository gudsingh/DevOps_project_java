@Library('my-shared-library') _

pipeline {

    agent any
        
        stages{
            stage ('Git Checkout'){
                steps {
                    gitCheckout(
                        branch: "master",
                        url: "https://github.com/gudsingh/DevOps_project_java.git"
                    )
                    
                }
            }
            stage ('Maven: Unit Test '){
                steps {
                    script {

                        mvnTest()
                    }
                    
                }
            }

        }
 
}