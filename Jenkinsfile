node{
    stage('Build'){
        def mavenImage = docker.image('maven:3.5.3-jdk-10-slim')
        mavenImage.pull()
        mavenImage.inside('-e someEnv=dev',{
            sh 'mvn -v'
        })
    }
}