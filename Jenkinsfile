node2 {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */
        
        cleanWs()
        echo "Clone repository"
        checkout scm
    }

    stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */

        app = docker.build("getintodevops/hellonode")
    }
}
