Jenkinsfile (Declarative Pipeline)
pipeline {
    stages {
        stage('build') {
            steps {
                script 
                  sh 'scope launch'
                  def root = tool name: 'Go 1.14', type: 'go'
                  withEnv(["GOPATH=${env.WORKSPACE}/go", "GOROOT=${root}", "GOBIN=${root}/bin", "PATH+GO=${root}/bin"]) {
                        sh "mkdir -p ${env.WORKSPACE}/go/src"
            }
        }
    }
}
