pipeline {

    agent any

    stages {
        stage ("Inicial"){
            steps {
                echo 'iniciando a pipeline'
            }
        }

        stage('build') {
            cmd_exec('echo "Buils starting..."')
            cmd_exec('echo "dir /a /b"')
        }

        def cmd_exec(command) {
            return bat(returnStdout: true, script: "${command}").trim()
        }
    }
}
