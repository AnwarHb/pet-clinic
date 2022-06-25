pipeline {
    agent any
    // added a comment to check jenkins-github trigger
    // comment // 
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
