node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'docker-hub-credentials') {

        def customImage = docker.build("tviles/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
