node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("juned171/dockerjenkins17")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
