pipeline {
    agent any

    tools {
    jdk 'JAVA_HOME'
    maven 'M2_HOME'
}


    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Achref-Neji-07/Devops.git'
            }
        }

        stage('Compile Stage') {
            steps {
                bat 'mvn clean compile'
            }
        }
    }
}
