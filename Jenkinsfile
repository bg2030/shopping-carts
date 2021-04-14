pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'Maven 3.6.3' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is the build job'
                sh 'uptime'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'uptime'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'uptime'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}

