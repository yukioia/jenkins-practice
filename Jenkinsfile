pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Сборка приложения...'
                sh 'echo "Build stage completed"'
            }
        }
        stage('Test') {
            steps {
                echo 'Тестирование приложения...'
                sh 'echo "Test stage completed"'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Деплой на стейджинг...'
                sh 'echo "Deployed to staging"'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Деплой на продакшн...'
                sh 'echo "Deployed to production"'
            }
        }
    }
    post {
        always {
            echo 'Пайплайн завершён'
        }
        success {
            echo 'Сборка прошла успешно'
        }
        failure {
            echo 'Сборка провалилась'
        }
    }
}
