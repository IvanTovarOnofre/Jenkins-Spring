pipeline{
    agent any
    stages {
        stage('Build'){
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Test'){
            steps {
                sh 'mvn test'
            }
        }

        stage('Deploy'){
           steps {
                echo "Desplegando..."
           }
        }
    }

    post{
        always{
            echo "Siempre"
        }
        success{
            echo "Exito"
        }
        failure{
            echo "Fallo"
        }
    }
}