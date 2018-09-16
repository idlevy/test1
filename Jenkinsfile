pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'ed  -i  "s/ido\ 7/row\ 333/g"\ ./file1'
               sh "env"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh " echo ${params.param1}"
                sh 'ed  -i  "s/ido\ 7/row\ 333/g"\ ./file1' 

            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
