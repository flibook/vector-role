pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                dir('vector-role') {
                    git credentialsId: 'c06a7f9a-4ea8-4a9b-b19b-5b4fef5c5a33', url: 'git@github.com:/flibook/vector-role.git'
                }
            }
        }
        stage('Molecule') {
            steps {
                dir('vector-role') {
                    sh 'molecule --version'
                    sh 'molecule test'
                }
            }
        }
    }
}
