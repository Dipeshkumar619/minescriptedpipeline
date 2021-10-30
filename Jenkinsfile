node{
    stage('Build'){
		checkout([$class: 'GitSCM', 
		branches: [[name: 'dockerfile']], 
		extensions: [], 
		userRemoteConfigs: [[credentialsId: 'githubapi', url: 'https://github.com/Dipeshkumar619/minescriptedpipeline.git']]])
        
        def myCustomUbuntuImage = docker.build("my-ubuntu:latest")
        mycustomUbuntuImage.inside{
            sh 'cat /etc/lsb-release'
        }


    }
}