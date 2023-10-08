pipeline {

    agent any

    stages {
        stage ("Inicial"){
            
            steps {
                powershell 'Write-Output "Hello, World"'
                powershell 'dir "Program Files (x86)/Nmap/"'
            }
        }
    }
}
