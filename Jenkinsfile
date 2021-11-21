pipeline { 
agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/maheedhar1208/jenkins.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x Fib.py"
                sh "./Fib.py"
            }
        }
     stage('Test Code') {
            steps {
                sh "chmod u+x Test.py"
                sh "./Test.py"
            }
        }
    } 
}
