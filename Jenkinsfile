pipeline {
    agent any

    stages{       
        stage('SonarQubeanalysis') {
            steps{
                script {
                    scannerHome = tool 'sonarscanner'
                    // La herramienta aquí es obtener la ruta del complemento instalado automáticamente directamente en función del nombre
                }
                withSonarQubeEnv('sonarqube') {
                    sh "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=TryPl"
                }
                //TRYYYYYYYYYYYYYYYYY!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
            }
        }
        stage('Hello'){
            steps {
                echo 'Hello, JDK'
            }
        }
    }
}
//try
