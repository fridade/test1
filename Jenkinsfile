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
                echo $NAME           // there is no var exchange within stages
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
                sh '''
                echo $NODE_NAME
                echo $NODE_LABELS
                echo $WORKSPACE
                echo $JENKINS_HOME
                echo $JENKINS_URL
                '''
            }
        }
















    }









}
