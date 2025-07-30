pipeline{
    agent any
    tools {
        maven 'Maven 3.3.11'
        jdk 'jdk8'
    }
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