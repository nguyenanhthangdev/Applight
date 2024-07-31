pipeline {
    agent any
    stages{
        stage('Clone') {
            steps {
                git credentialsId: 'github', url: 'https://github.com/nguyenanhthangdev/Applight.git'
            }
        }
    }
}