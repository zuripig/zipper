pipeline {
    agent any
    stages {
        stage('zip') {
            steps {
                sh 'echo "hello"'
                zip archive: true, dir: '', glob: '', zipFile: 'testzip.zip'
                archiveArtifacts artifacts: 'testzip.zip', onlyIfSuccessful: true
                sh 'rm deleteme.git'
            }
        }
    }
}
