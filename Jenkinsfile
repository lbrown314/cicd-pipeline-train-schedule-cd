pipeline {
    agent any
    stages {
        stage('Pre-Test 1') {
            steps {
                echo 'Running Pre-Test 1'
            }
        }
        stage('Pre-Test 2') {
            steps {
                echo 'Running Pre-Test 2'
                exit 1 
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
        stage('Post-Test 3') {
            steps {
                echo 'Running Post-Test 3'
            }
        }
        stage('Post-Test 4') {
            steps {
                echo 'Running Post-Test 5'
            }
        }
        stage('Post-Test 5') {
            steps {
                echo 'Running Post-Test 5'
            }
        }
        stage('Deploying to staging') {
            steps {
                echo 'Deploying to staging'
            }
        }
        stage('Deploying to prod') {
            steps {
                echo 'Deploying to prod'
            }
        }
    }
}
       
