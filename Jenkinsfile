pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo "Repository cloned successfully"
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                scp -i /home/ubuntu/key.pem -o StrictHostKeyChecking=no index.html ubuntu@13.234.231.229:/var/www/html/
                '''
            }
        }

    }
}
