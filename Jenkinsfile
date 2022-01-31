node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {
        def customImage = docker.build("test/dockerapp")
        customImage.push()
    }
}