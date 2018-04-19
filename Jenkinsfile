#!/usr/bin/env groovy Jenkinsfile
node{
    def gradleHome = tool 'gradle4.7'
    env.PATH = "${gradleHome}/bin:${env.PATH}"
}
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'gradle build --info'
            }
        }
        stage('Test') {
             steps {
                    sh 'gradle test --info'
             }
         }
    }
}
