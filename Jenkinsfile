pipeline {
    agent any
    environment{
        NOMBRE='Romina'
        APELLIDO='Mendez'
        secret=credentials('test') 
    }
    stages{
        stage('checkout'){
            steps{
                echo 'checkout'
                echo 'variables'
                sh 'echo $NOMBRE $APELLIDO'
                sh 'echo secrets github: $secret'
            }
        }
        stage('install'){
            steps{
                echo 'install dependencies'
            }
        }
        stage('test'){
            steps{
                echo 'test'
            }
        }
        stage('deploy'){
            steps{
                echo 'deploy'
            }
        }
    }
    
}
