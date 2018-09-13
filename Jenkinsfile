pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
               sh "env"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh " echo ${params.param1}" 
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
