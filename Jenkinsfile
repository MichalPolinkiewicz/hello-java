node {
    def projectName = "Java-Test-App"

    stage('Build') {
        try {
            bat "mvn clean install"
        } catch (ex) {
            echo "application build failed"
        }
    }
}