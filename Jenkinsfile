pipeline {

    agent any

    stages {
        stage ("Inicial"){
            
            steps {
                powershell 'Write-Output "Hello, World"'
                powershell 'cd "/Program Files (x86)/Nmap"'
                powershell 'dir'
            }
        }
    }
}
