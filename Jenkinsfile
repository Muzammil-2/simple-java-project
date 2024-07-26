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
                git branch: 'qa', credentialsId: 'GITHUB_CREDENTIALS_1', url: 'https://github.com/quadrimuzammil/maven-web-application.git'
            }
        }
    }
}   