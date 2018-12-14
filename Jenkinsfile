pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                echo 'Starting the Gradle Build!!!!....'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
