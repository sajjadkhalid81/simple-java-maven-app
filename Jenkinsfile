pipeline{
    agent{
        label 'agentx'
    }
     tools {
        maven 'maven1' 
    }
    stages{
        stage('checkout'){
            steps{
            checkout scm
            }
        }
        stage('build'){
            steps{
                sh 'mvn clean install'
            }
        }
        stage('post-build'){
            steps{
                echo "this is post build message "
            }
        }
        
    }
}
