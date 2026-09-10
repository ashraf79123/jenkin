pipeline{
    agent any
    
    tools{
        maven "mymaven"
    }
    
    stages{
        stage('checkout Code')
        {
            steps{
            git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
        stage('compile code'){
            steps{
                echo "compling the code ..."
                sh 'mvn compile'
            }
        }
        stage('Test code'){
            steps{
                echo "testing using junit"
                sh 'mvn test'
            }
        }
        stage('BuildCode'){
            steps{
            echo "building...."
            sh 'mvn package'
            }
        }
    }
}
