@Library('jenkins@main') _
import org.opstree.Utils

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
                    sayHello('Abhinav')   // from vars/sayHello.groovy
                    def utils = new Utils(this)
                    utils.runSampleMethod('Abhinav123') // from src/org/opstree/Utils.groovy
                }
            }
        }

        stage('Completion') {
            steps {
                echo "Shared library functions executed successfully!"
            }
        }
    }
}
