pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                echo "========executing building stage========"
                sh "./gradlew build --no-daemon"
                archiveArtifacts artifacts: "dist/trainSchedule.zip"
            }
        }
    }
}