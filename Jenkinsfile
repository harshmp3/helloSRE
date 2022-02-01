node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {
        def customImage = docker.build("test")
        customImage.push()
    }
}