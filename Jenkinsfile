pipeline {
    agent any

    stages {
        stage('Get latest source code') {
            steps {
                git 'https://github.com/shivanitejale/Jenkins_multijob_pipeline_code.git'
            }
        }
        stage('Compile ') {
            steps {
                sh 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
