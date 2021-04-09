#!/usr/bin/env groovy
// The above line is used to trigger correct syntax highlighting.

pipeline {
    agent { docker { image 'golang:1.13' } }
    stages {
        stage('build') {
            steps {
                sh 'go version'
            }
        }
    }
}