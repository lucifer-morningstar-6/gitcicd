pipeline {
    agent any
    stages {
        stage('Check File') {
            steps {
                script {
                    def content = readFile('a.txt')
                    if (content.contains("sss")) {
                        echo "PASS"
                    } else {
                        error "FAIL"
                    }
                }
            }
        }
    }
}
