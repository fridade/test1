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
                echo $COUNTRY       // this is call in  stage variable and this var cant be print else where
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
