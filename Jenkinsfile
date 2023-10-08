pipeline {

    agent any

    stages {
        stage ("Inicial"){
            
            steps {
                powershell 'Write-Output "Hello, World"'
                powershell '."/Program Files (x86)/Nmap/nmap.exe" -sV localhost'
            }
        }
    }
}
