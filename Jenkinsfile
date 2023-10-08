pipeline {

    agent any

    stages {
        stage ("Inicial"){
            steps {
                echo 'iniciando a pipeline'
            }
            steps {
                nmap -sV localhost
            }
        }
    }
}
