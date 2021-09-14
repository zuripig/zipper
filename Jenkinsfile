pipeline {
    agent any
    stages {
        stage('zip') {
            steps {
                sh 'echo "hello jemma"'
                zip archive: true, dir: '', glob: '', zipFile: 'testz.zip'
            }
        }
    }
}
