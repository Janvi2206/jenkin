pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the code using a build automation tool (e.g., Maven)...'
                echo 'Recommended tool: Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit tests and integration tests...'
                echo 'Recommended test automation tool: JUnit (for unit tests), Selenium (for integration tests)'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Integrating a code analysis tool (e.g., SonarQube) to analyze the code...'
                echo 'Recommended tool: SonarQube'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Performing a security scan on the code...'
                echo 'Recommended tool: OWASP ZAP (Zed Attack Proxy)'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying the application to a staging server (e.g., AWS EC2 instance)...'
                echo 'Recommended deployment tool: Jenkins Pipeline (with AWS CodeDeploy plugin)'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on the staging environment...'
                echo 'Recommended tool: Apache JMeter'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying the application to a production server (e.g., AWS EC2 instance)...'
                echo 'Recommended deployment tool: Jenkins Pipeline (with AWS CodeDeploy plugin)'
            }
        }
    }
    post {
        success {
            // Cleanup steps, if any
            emailext body: 'sent successfully ', subject: 'test email', to: 'janvi4794.be22@chitkara.edu.in'
        }
    }
}

