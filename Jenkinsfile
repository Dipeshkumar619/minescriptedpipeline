node{
    stage('Build'){
        ws('/var/lib/jenkins/workspace/nodeDockerCustomWorkspace') {
            def maven.Image =  docker.withRegistry('https://quay.io','quay.io'){
                docker.image('quay.io/dipesh_gupta_ak/myfirstrepo:latest').inside{
                    sh 'printenv'
                }
            }


        }

    }
}