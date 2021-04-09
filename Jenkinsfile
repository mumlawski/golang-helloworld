#!/usr/bin/env groovy
// The above line is used to trigger correct syntax highlighting.

pipeline {
    agent { docker { 
          image 'golang:1.13'
          args '-v c:/Michal/jenkins/workspace/test123_master:/var/jenkins_home/workspace/test123_master'
          args '-u 1000:1000'
          reuseNode true 
          } }
    stages {
        stage('build') {
            steps {
                sh 'go version'
            }
        }
    }
}