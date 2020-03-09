Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker { image 'go:1.4' } }
    stages {
        stage('build') {
            steps {
                sh 'jenkins -ex scope.sh launch'
            }
        }
    }
}
