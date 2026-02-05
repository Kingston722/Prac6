pipeline {
    agent any

    tools {
        jdk 'JDK17'
    }

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Kingston722/Prac6.git'
            }
        }

        stage('Compile Java') {
            steps {
                bat '''
                    javac Prac6.java
                '''
            }
        }

        stage('Run Program') {
            steps {
                bat '''
                    java Prac6
                '''
            }
        }
    }
}
