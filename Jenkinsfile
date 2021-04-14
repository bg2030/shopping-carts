pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'maven' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is the build job'
                sh 'pom.xml compile'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'pom.xml clean test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'pom.xml package -DskipTests'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}

