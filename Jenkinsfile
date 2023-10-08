pipeline {

    agent any

    stages {
        stage ("Inicial"){
            
            steps {
                powershell 'Write-Output "Hello, World"'
                powershell 'nmap -sV localhost'
                
            }
        }
    }
}
