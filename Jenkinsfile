pipeline {
    agent any
    tools {
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
    stages {
        stage('GIT') {
            steps {
                git branch: 'master',
                url: 'https://github.com/ziedtabib/projet_timesheet.git'
            }
        }
        stage('Compile') {
            steps {
                sh 'mvn clean compile'
            }
        }


}
