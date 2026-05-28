pipeline {
    agent {
        label 'AGENT-1'
    }
    // Build
    stages{
        stage('build'){
            steps{
                script{

                    echo "Building..." 
                    }
                 }
        }
        stage('test'){
            steps{
               script{
                    
                    echo "Testing..."
                }
            }
        }
        stage('deploy'){
            steps{
                script{
                    
                    echo "Deploying..."
                }
            }
        }
    }

   
   post {
      always{
        echo "I will always say hello"
        deleteDir()
      }
      success{
        echo "Hello Success"
      }
      failure{
        echo "Hello Failure"
      }

    
   } 

}