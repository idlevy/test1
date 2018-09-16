pipeline {
    agent any

    parameters {
       // booleanParam(
       //     name:'scale_only',
       //     defaultValue:"${scale_only:"true"}",
       //     description: "scale pods up or down only. no configuration update.")
       string(
           name: 'old_version',
           defaultValue:"${1234}",
           description: ".")

       string(
           name: 'new_version',
           defaultValue:"0.0.0.0",
           description: "NEW VERSION")
           }


    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo $old_verison
                echo $new_version
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
                  echo $new_version

              //  sed  -i  "s/$version/$new_version/g" ./version
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
