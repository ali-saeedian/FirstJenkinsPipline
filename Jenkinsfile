pipeline{
    agent any
    stages{
        stage('Checkout') {
            steps{
                echo 'Starting Checkout from branch master'
                git branch:'master' , url:'https://github.com/ali-saeedian/FirstJenkinsPipline.git'
                echo 'Checkout completed'
            }
            }
              stage('Restore') {
            steps{
                echo 'Starting package restore'
                bat 'dotnet restore'
                echo 'Restore completed Successfuly'
            }
            }
                   stage('Build') {
            steps{
                echo 'Starting Build prossess'
                bat 'dotnet build'
                echo 'build completed Successfuly'
            }
            }
                    stage('test') {
            steps{
                echo 'Starting unit test'
                bat 'dotnet test'
                echo 'tests completed Successfuly'
            }
            }
        }
        }
    

