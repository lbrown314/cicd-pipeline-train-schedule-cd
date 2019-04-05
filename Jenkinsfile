pipeline {
    agent any
    stages {
        stage('Pre-Test') {
            steps {
                echo 'Running Pre-Test'
            }
        }
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        stage('Post-Test 1') {
            steps {
                echo 'Running Post-Test 1'
            }
        }
        stage('Post-Test 2') {
            steps {
                echo 'Running Post-Test 2'
            }
        }
    }
}
       
