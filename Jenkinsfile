pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building branch: ${env.BRANCH_NAME}"
              echo "This is testing for multi branch do build"
                
                // Example: sh 'npm install' or sh 'mvn package'
            }
        }
        stage('Test') {
            steps {
                echo "Testing branch: ${env.BRANCH_NAME}"
              echo "This is main"
                // Example: sh 'npm test' or sh 'mvn test'
            }
        }
        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                echo "Deploying branch: ${env.BRANCH_NAME}"
                echo "this is updated one"
                // Example: sh './deploy.sh'
            }
        }
    }
}
