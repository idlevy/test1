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
                //sh " echo ${params.param1}"
                sh 'ls'
                sh 'pwd'
                sh 'sed  -i  "s/ido 7/row 333/g" ./file1'

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
