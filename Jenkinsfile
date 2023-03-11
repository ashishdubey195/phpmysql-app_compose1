pipeline{

    agent any
    stages{
    stage('SCM Checkout')
    {
        steps{
        git 'https://github.com/purdueorg1/phpmysql-app_compose.git'
    }
    }
    
    stage('Run Docker Compose File')
    {
        steps{
        sh 'sudo docker compose build'
        sh 'sudo docker compose up -d'
    }
    }
}
}
