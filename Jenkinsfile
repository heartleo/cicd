pipeline {
   agent any

   stages {
      stage('pull code') {
         steps {
            echo 'pull code'
            git branch: 'main', credentialsId: 'heartleo-github-token', url: 'https://github.com/heartleo/cicd.git'
         }
      }
      stage('build code') {
         steps {
            echo 'build code'
            sh '''cd cmd/pipeline
pwd
ls -al'''
         }
      }
      stage('deploy project') {
         steps {
            echo 'deploy project'
         }
      }
   }
}
