pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo '======================================'
                echo 'STAGE 1: BUILD'
                echo '======================================'
                echo 'Tool Used: Apache Maven'
                echo 'Purpose: Compile source code and package application artifacts.'
            }
        }

        stage('Unit and Integration Testing') {
            steps {
                echo '======================================'
                echo 'STAGE 2: UNIT AND INTEGRATION TESTING'
                echo '======================================'
                echo 'Tools Used: JUnit and Selenium'
                echo 'Purpose: Execute automated unit and integration tests.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo '======================================'
                echo 'STAGE 3: CODE ANALYSIS'
                echo '======================================'
                echo 'Tool Used: SonarQube'
                echo 'Purpose: Analyse code quality and maintain coding standards.'
            }
        }

        stage('Security Scan') {
            steps {
                echo '======================================'
                echo 'STAGE 4: SECURITY SCAN'
                echo '======================================'
                echo 'Tool Used: OWASP Dependency Check'
                echo 'Purpose: Detect known security vulnerabilities and CVEs.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo '======================================'
                echo 'STAGE 5: DEPLOY TO STAGING'
                echo '======================================'
                echo 'Tool Used: AWS CodeDeploy'
                echo 'Purpose: Deploy application to staging environment.'
            }
        }

        stage('Integration Testing on Staging') {
            steps {
                echo '======================================'
                echo 'STAGE 6: INTEGRATION TESTING ON STAGING'
                echo '======================================'
                echo 'Tools Used: Selenium and Postman'
                echo 'Purpose: Validate application functionality in staging.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo '======================================'
                echo 'STAGE 7: DEPLOY TO PRODUCTION'
                echo '======================================'
                echo 'Tool Used: AWS EC2'
                echo 'Purpose: Deploy verified application to production.'
            }
        }
    }

    post {

        success {
            echo 'Pipeline executed successfully.'
        }

        failure {
            echo 'Pipeline execution failed.'
        }

        always {
            echo 'Pipeline execution completed.'
        }
    }
}