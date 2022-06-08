node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("mwar8205/node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}