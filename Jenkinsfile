// Declarative //
pipeline {
    agent any
    
 //   environment {
   //     sonarqubeScannerHome = tool name:'SonarScannerTest'

   // }

    stages {

        stage('Build') {
            steps {
                echo 'Building..'
                sh 'cd webdemo && ./gradlew build -x test'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'cd webdemo && ./gradlew test || true'
              //  junit '**/target/*.xml'
            }
        }

        
        
     
        
    }
}
