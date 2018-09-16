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
                sh '''
                  echo $version
                  new_version=$((version +1))

                sh 'sed  -i  "s/$version/$new_version/g" ./ version'
                '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
