pipeline {
    agent any
    stages {
        stage('Stage release') {
            steps {
                sh """
                npm run release
                """
            }
        }
        stage('Stage push') {
            steps {
                sh """
                npm run release:tags
                """
            }
        }
    }
}