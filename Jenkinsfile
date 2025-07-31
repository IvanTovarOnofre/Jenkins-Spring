pipeline{
    agent any
    stages {
        stage('Build'){
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Build'){
            steps {
                sh 'mvn test'
            }
        }
        stage('Build'){
           steps {
                echo 'Desplegando...'
           }
        }
    }

    post{
        always{
            echo 'Siempre'
        }
        success{
            echo "Exito"
        }
        failure{
            echo "Fallo"
        }
    }
}