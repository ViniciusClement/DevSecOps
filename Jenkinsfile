pipeline {

    agent any

    stages {
        stage ("DAST"){
            
            steps {
                powershell 'Write-Output "Hello, World"'
                powershell '."/Program Files (x86)/Nmap/nmap.exe" -sV -sC -A -O localhost '
                python "C:/Program Files/sqlmap/sqlmap.py" --help 
            }
        }
    }
}
