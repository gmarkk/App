pipeline   
    agent{
        label "jenkins-agent"
    }
    tools {
        jdk 'Java17'
        maven 'Maven3'

    }
    stages{
        stage("Cleanup Workspace"){
            steps {
                cleanWs()

            }
        }    

        stage("Checkout from SCM"){
           steps{
            git branch: 'main',crendtialsId: 'github', url: 'https://github.com/gmarkk/App'
        }
        
    }
}
