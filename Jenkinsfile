pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'Maven' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is the build job'
                sh 'compile'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'clean test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'package -DskipTests'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}

