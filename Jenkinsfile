pipeline{
    agent any
    ## A simple pipeline to build and test a .NET project
    stages{
        stage('Restore the project'){
            steps{
                bat 'dotnet restore'
            }
        }
        stage('Build the project'){
            steps{
                bat 'dotnet build --no-restore'
            }
        }
        stage('Run the tests'){
            steps{
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
        
    }
}