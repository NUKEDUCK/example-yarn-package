#!/usr/bin/env groovy

pipeline {
  agent {
    label {
      label 'noobjs12'
    }
  }
    stages {
        stage('Build') {
            steps {
                sh 'nodejs --version'
                sh 'yarn install'
            }
        }
        stage('Test') {
            steps {
                sh 'nodejs --version'
                sh 'yarn run test'
            }
        }
    }
    post {
         success {
            echo 'I succeeeded!'
        }
        failure {
            echo 'I failed :('
        }

    }
}
