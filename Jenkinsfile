pipeline {
    agent any
    stages {
        stage('zip') {
            steps {
                sh 'echo "hello"'
                //zip archive: true, dir: '', glob: '', zipFile: 'testzip.zip'
                zip -r test.zip zipPipe_main
            }
        }
    }
}
