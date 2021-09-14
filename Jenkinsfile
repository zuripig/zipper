pipeline {
    agent any
    stages {
        stage('zip') {
            steps {
                sh 'echo "hello"'
                sh 'rm -rf .git' 
                zip archive: true, dir: '', glob: '', zipFile: 'testzip.zip'
                archiveArtifacts artifacts: 'testzip.zip', onlyIfSuccessful: true
            }
        }
    }
}
