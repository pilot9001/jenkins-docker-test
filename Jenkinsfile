pipeline {
    agent {
        docker {
            image 'python'
            label 'generic'
        } //docker
    } //agent
    stages {
        stage("Run Hello World") {
            steps {
                sh """
                    python helloworld.py
                """
            } //steps
        } //stage
    } //stages
} //pipeline