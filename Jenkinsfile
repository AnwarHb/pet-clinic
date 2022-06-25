pipeline {
    agent any
    // added a comment to check jenkins
    stages {
       
        //
        stage("Build") {
            steps {
                sh "mvn clean package"
            }
        }
        //
        
        stage("Save Artifact") {
            steps {
                archiveArtifacts artifacts: 'target/*.jar', followSymlinks: false
            }
        }
    }
}
