#!/usr/bin/env groovy
// The above line is used to trigger correct syntax highlighting.

pipeline {
    agent { docker { 
          image 'golang:1.13'
          args '-v /var/jenkins_home:/var/jenkins_home' 
          } }
    stages {
        stage('build') {
            steps {
                sh 'go version'
            }
        }
    }
}