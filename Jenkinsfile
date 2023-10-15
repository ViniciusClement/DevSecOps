pipeline {

    agent any

    stages {
        
        stage ("Environmet"){
            environment {
                user = "Vinicius"        
                echo "Este é o meu usuario $user"
            }
        }

        stage ("SAST"){
            steps {
                powershell 'Write-Output "Iniciando análise SAST..."'
                powershell '."/xampp/htdocs/horusec.exe" start -p .'
            }
        }
        
        stage ("DAST"){
            
            steps {
                powershell 'Write-Output "Iniciando análise DAST..."'
                powershell '."/Program Files (x86)/Nmap/nmap.exe" -sV -sC -A -O localhost '
                powershell '."C:/Program Files (x86)/Python/python.exe" "/Program Files/sqlmap/sqlmap.py" -u http://127.0.0.1 --crawl=1 --random-agent --batch --forms --threads=5 --level=5 --risk=3'
            }
        }
    }
}

