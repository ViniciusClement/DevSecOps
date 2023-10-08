pipeline {

    agent any

    stages {
        stage ("Inicial"){
            steps {
                echo 'iniciando a pipeline'
            }
        }
    }

    stages {
        stage ("DAST"){
            steps {
                nmap -sV localhost
            }
        }
    }


}