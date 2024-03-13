pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Add your build steps here
                //bat 'echo "Building..."'
                sh "mvn clean install"
                // You can replace the above line with your actual build commands
            }
        }
    }
    post {
        success {
            // Cleanup steps, if any
            emailext body: 'sent successfully ', subject: 'test email', to: 'tjanvi2206@gmail.com'
        }
    }
}
