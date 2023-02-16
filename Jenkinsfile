pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o pes2ug20cs446.exe new.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './pes2ug20cs447.exe'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
