pipeline {
    agent any
    tools{
        java "myjava"
        maven "mymaven"
    }
    stages {
        stage('Hello') {
            steps {
                script{
                echo 'Hello World Vani'
            }
        }
        }
        stage('COMPILE') {
            steps {
                script{
                echo 'COMPILE THE CODE'
                sh 'mvn compile'
            }
        }
        }
        stage('UNITEST') {
            steps {
                script{
                echo 'RUN THE UNIT TC'
                sh 'mvn test'
            }
        }
        }
        stage('PACKAGE') {
            steps {
                script{
                echo "PACKAGE THE CODE"
                sh 'mvn package'
            }
        }
        }
    }
}
