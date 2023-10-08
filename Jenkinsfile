pipeline {

    agent any

    stages {
        stage ("DAST"){
            
            steps {
                powershell 'Write-Output "Hello, World"'
                //powershell '."/Program Files (x86)/Nmap/nmap.exe" -sV -sC -A -O localhost '
                //powershell '."/Program Files (x86)/sqlmap/sqlmap.ps1"'     
                powershell '"C:/Program Files (x86)/Python/python.exe"'
            }
        }
    }
}

