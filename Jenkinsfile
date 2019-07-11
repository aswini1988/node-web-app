#!/bin/groovy
pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
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