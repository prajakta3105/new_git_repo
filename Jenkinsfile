pipeline {
    agent any
    stages {
        /* "Build" and "Test" stages omitted */

        stage('Deploy - Staging') {
            steps {
                git 'https://github.com/newuser31/test-git-repo.git'
               
            }
        }

        stage('Sanity check') {
            steps {
                input "Does the staging environment look ok?"
            }
        }

        stage('Deploy - Production') {
            steps {
                echo "Deployment completed successfully!!!!!!!"
            }
        }
    }
}
