pipeline{
    agent any

    stages{

        stage('Checkout SCM'){
            steps{
                checkout scm
            }
        }

        stage('build'){
            bat "dotnet build"
        }

        stage('Run tests'){
            steps{
                bat "dotnet test"
            }

        }
    }
}