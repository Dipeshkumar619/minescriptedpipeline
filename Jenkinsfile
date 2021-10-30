node{
    stage('Build'){
        ws('/var/lib/jenkins/workspace/nodeDockerCustomWorkspace') {
            def mavenImage =  docker.withRegistry('https://quay.io','dipesh_gupta_ak'){
                docker.image('quay.io/dipesh_gupta_ak/myfirstrepo:latest').inside {
                    sh 'printenv'
                }
            }


        }

    }
}