pipeline {

    agent any

    stages {
        stage ("DAST"){
            
            steps {
                powershell 'Write-Output "Hello, World"'
                powershell '."/Program Files (x86)/Nmap/nmap.exe" -sV -sC -A -O localhost '
                powershell 'python "C:/Program Files/sqlmap/sqlmap.py" -u http://127.0.0.1  --crawl=1 --random-agent --batch --forms --threads=5 --level=5 --risk=3'
            }
        }
    }
}
