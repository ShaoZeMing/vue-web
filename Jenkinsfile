#!/usr/bin/env groovy
pipeline {
    agent any
    environment {
         AN_ACCESS_KEY = credentials('zeming')
         }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                echo AN_ACCESS_KEY
                npm install

            }
        }
        stage('Test') {
            steps {
                echo 'Hello This is Hello'
                npm run serve

            }
        }
        stage('Deploy') {
            steps {
                echo 'Hello This is Deploy'
                npm run build
            }
        }
    }
}

