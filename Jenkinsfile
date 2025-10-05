pipeline {
    agent any

    stages {
        stage('Initialization') {
            steps {
                echo "Pipeline execution started in the application repository."
            }
        }

        stage('Shared Library Execution') {
            steps {
                script {
                    sayHello('Abhinav Sikarwar')
                }
            }
        }
    }
}
