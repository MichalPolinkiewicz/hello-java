node {
    def projectName = "Java-Test-App"

    stage('Build') {
        try {
            bat "mvn clean install"
        } catch (ex) {
            notifyFail("${projectName} build failed")
           
        }
    }
    stage('Stage 2') {
        echo "stage 2 executed"
    }
    stage('Stage 3') {
        echo "stage 3 executed"
    }
}

def notifyFail(msg = null) {
        error(msg)
}
