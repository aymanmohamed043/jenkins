pipeline {
    agent {
        label 'agent-0'
    }

    tools {
        maven 'mvn-3-5-2'
    }

    // stages {
    //     stage('Check SCM') {
    //         steps {
    //             git branch: 'main', url: 'https://github.com/Hassan-Eid-Hassan/python-iti'
    //         }
    //     }
        stage('Build') {
            steps {
                sh 'mvn package install'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
