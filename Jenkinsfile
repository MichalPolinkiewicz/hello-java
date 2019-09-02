node {
    def projectName = "Java-Test-App"

    stage('Build') {
        try {
            bat "mvn clean install"
        } catch (ex) {
            echo "application build failed"
            currentBuild.result = 'FAILED'
            return;
        }
    }
    stage('Stage 2') {
        echo "stage 2 executed"
    }
}
