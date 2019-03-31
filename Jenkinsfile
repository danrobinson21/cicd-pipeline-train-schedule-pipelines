pipeline {
    agent any
    stages {
        stage ('build') {
            steps {
                echo 'Building code'
                sh ./gradlew gradle.build --no-daemon
                achiveArtefacts artefacts: 'dist/trainschedlue.zip'
            }
        }
    }
}