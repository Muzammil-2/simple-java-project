pipeline {
    agent any
    tools {
  maven 'Maven 3.8.6'
}

environment {
  buildNumber = "BUILD_NUMBER"
}

    stages {
        stage('Git_Clone') {
            steps {
                git credentialsId: 'Github_Id', url: 'https://github.com/Muzammil-2/simple-java-project.git'
            }
        }

         stage('Build_Codes') {
            steps {
                sh 'mvn clean package'
            }
        }
    
    
    
    }
}   