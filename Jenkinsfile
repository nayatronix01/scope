Jenkinsfile (Declarative Pipeline)
pipeline {
    stages {
        stage('build') {
            steps {
                script 'scope launch'
                 def root = tool name: '1.4', type: 'go'
                withEnv(["GOPATH=${env.WORKSPACE}/go", "GOROOT=${root}", "GOBIN=${root}/bin", "PATH+GO=${root}/bin"]) {
                        sh "mkdir -p ${env.WORKSPACE}/go/src"
            }
        }
    }
}
