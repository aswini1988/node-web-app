#!/bin/groovy

library identifier: 'jenkins-shared-lib@master',retriever: modernSCM([$class: 'GitSCMSource',
	remote: 'https://github.com/aswini1988/jenkins-shared-lib.git',
	credentialsId: 'dockerAswini'])

pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                new StartBuild().build()
                echo "This is a Build stage"
                sh "pwd"
            }
        }
        stage('Test') { 
            steps {
                echo "This is a Test stage"
                sh """
                    pwd
                    ls -la
                """
            }
        }
        stage('Deploy') { 
            steps {
                echo "This is a Deploy stage"
            }
        }
    }
}