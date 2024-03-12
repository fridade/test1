pipeline {
    agent any
    environment {
     NAME = "FRITZ"           // GLOBAL VARIABLE CAN BE USE AT ALL THE STAGES
     COUNTRY = "CAMEROON"
    }





    stages {



        stage('build') {
            steps {
                sh '''
                echo $NAME
                echo $COUNTRY
                '''
            }
        }


        stage('verify') {
            steps {
                sh '''
                app=canary
                echo $app
                '''
            }
        }


        stage('deploy') {
            steps {
                echo 'Hello World'
            }
        }
















    }









}
