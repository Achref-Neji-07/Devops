pipeline {
    agent any

    tools {
        jdk    'JAVA_HOME'   // même nom que dans Manage Jenkins > Global Tool Configuration
        maven  'M2_HOME'
    }

    stages {
        stage('GIT') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/hwafa/timesheetproject.git'
            }
        }

        stage('Compile Stage') {
            steps {
                // tu es sur Windows, donc utilise bat et pas sh
                bat 'mvn clean compile'
            }
        }
    }
}
