pipeline{
    agent any
    stages{
        stage('Build'){
           git url: 'https://github.com/IvanTovarOnofre/Jenkins-Spring.git'
            withMaven {
                sh "mvn clean verify"
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