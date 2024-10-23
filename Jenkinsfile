#!/usr/bin/env groovy

pipeline {
    agent {
        node {
            label 'Android_Builder_x64'    
        }
    }

    stages {
        
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
