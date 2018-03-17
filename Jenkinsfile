#!/usr/bin/env groovy

pipeline {

    agent { label 'Node01'
        }
    

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
		sh ' sudo apt-get install npm'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
    }
}
