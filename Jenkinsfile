pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Add your build steps here
                sh 'echo "Building..."'
                // You can replace the above line with your actual build commands
            }
        }
    }
    
    post {
        success {
            // Cleanup steps, if any
            emailext body: 'Email sent out from jenkins', subject: 'Test Email', to: 'janvi4794.be22@chitkara.edu.in'
        }
    }
}
