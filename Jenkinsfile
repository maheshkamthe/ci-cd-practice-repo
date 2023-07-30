pipeline {

    agent {
        node {
            label 'master'
        }
    }


    stages {

        stage('Build Code') {
            steps {
                echo "Building Code"
			}
        }

        stage('Unit Testing') {
            steps {
                echo "Running Unit Tests"
            }
        }

        stage('Code Analysis') {
            steps {
                echo "Running Code Analysis"
            }
        }

        stage('Build Deploy Code') {
            when {
                branch 'develop'
            }
            steps {
                echo "Building Artifact"
                echo "Deploying Code"
            }
        }

    }   
}
