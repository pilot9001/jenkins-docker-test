pipeline {
    agent {
        dockerfile {
            label 'generic'
        } //dockerfile
    } //agent
    stages {
        stage("Run Hello World") {
            steps {
                sh """
                    python helloworld.py
                """
            } //steps
        } //stage
        stage("Test request") {
            steps {
                sh """
                    python requestgoogle.py
                """
            }
        }
    } //stages
} //pipeline