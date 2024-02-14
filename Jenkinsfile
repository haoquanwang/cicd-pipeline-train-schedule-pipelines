pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifiacts artifiacts: 'dist/trainSchedule.zip'
            }
        }
    }
}