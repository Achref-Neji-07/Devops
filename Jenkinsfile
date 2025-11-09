pipeline {
    agent any

    tools {
    jdk 'JAVA_HOME'
    maven 'M2_HOME'
}


    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: ' https://github.com/hwafa/timesheetproject.git'
            }
        }

        stage('Compile Stage') {
            steps {
                bat 'mvn clean compile'
            }
        }
    }
}
