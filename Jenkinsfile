pipeline {
    agent any
    environment {
name = 'kishore'
BUILD_NAME = "********-${BUILD_NUMBER}********"
}
options {
    //timestamps()
    buildDiscarder(logRotator(numToKeepStr: '4'))
  }
    stages {
        stage('Buildversion') {
            steps {
                script {
                         currentBuild.displayName = env.BUILD_NAME
                       }
		    }
		}
        stage('Example') {
            steps {
                echo "**Running** ${env.BUILD_ID} **on** ${env.JENKINS_URL}"
            //    echo "my Job name is :${env.JOB_NAME} and ${BUILD_NUMBER}"
              //  echo "my name is :${name}"
              
             // echo "********************name***********************************"
            }
        }
        
        
    }
}
