pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'mvn clean install'
            }
        }
        stage('Test'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Deploy'){
            steps{
                echo "Simulando un despliegue"
            }
        }
    }

    post{
        always{
            echo 'Simpre'
        }
        success{
            echo "Exito"
        }
        failure{
            echo "Falla"
        }
    }
}