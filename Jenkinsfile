#!/usr/bin/env groovy

pipeline {
    agent {
        node {
            label 'Android_Builder_x64'    
        }
    }

    stages {
       // stage ('Checkout') {
       //     steps {
      //          sh 'printenv'
       //         checkout([$class: 'GitSCM', branches: [[name: params.get('GIT_BRANCH')]], doGenerateSubmoduleConfigurations: false, extensions: [], gitTool: 'Default', submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'tkachenko_github', url: 'https://github.com/Eugentk/webhook_jenkins.git']]])
   //         }
     //   }
        stage("Update server") {
        steps {
                sh 'ls -la'  
            }
        }
    }
post {
        always {
            echo 'Pipeline finished'
        }
        success {
            echo 'Pipeline script succeeded!'
        }
        unstable {
            echo 'Pipeline unstable :/'
        }
        failure {
            echo 'Pipeline script failure'
        }
        changed {
            echo 'Pipeline were different before...'
        }
    }
} 
