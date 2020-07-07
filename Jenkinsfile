pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                nodejs('node') {
                    git 'https://github.com/ChainzOwn-dev/postman-newman-jenkins.git'
                    // Run Maven on a Unix agent.
                    sh "npm install"
                    sh "npm run api-tests-production"
                }
            }
        }
    }
}
