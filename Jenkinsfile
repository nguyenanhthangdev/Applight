pipeline {
    agent any
    stages{
        stage('Clone') {
            steps {
                git credentialsId: 'github', url: 'https://github.com/nguyenanhthangdev/Applight.git'
            }
        }
        stage('Push Docker Hub') {
            steps {
                // This step should not normally be used in your script. Consult the inline help for details.
                withDockerRegistry(credentialsId: 'creds-dockerhub', url: '') {
                    // some block
                    // sh label: '', script: 'docker build -t nguyenanhthangdev/applight:latest .'
                    // sh label: '', script: 'docker push nguyenanhthangdev/applight:latest'

                    // sh label: '', script: 'docker build -t nguyenanhthangdev/applight:latest .'
                    sh label: '', script: 'docker pull nguyenanhthangdev/applight'
                }
            }
        }
    }
}