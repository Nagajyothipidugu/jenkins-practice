pipeline {
    agent {
        label 'AGENT-1'
    }
    // Build
    stages{
        stage('build'){
            steps{
                echo "Building..."
            }
        }
        stage('test'){
            steps{
                echo "Testing...."
            }
        }
        stage('deploy'){
            steps{
                echo  "Deploying......"
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