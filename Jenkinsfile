node {
    def projectName = "Java-Test-App"

    stage('Build') {
        try {
            bat "mvn clean install"
        } catch (ex) {
            echo "application build failed"
            currentBuild.result = 'ABORTED'
        }
    }
    stage('Stage 2') {
        echo "stage 2 executed"
    }
}
