pipeline{
    agent{
        label "master"
    }
    stages{
        stage("clone repo"){
            steps{
                //clean workspace before build
                cleanWs()
                sh '''
                 echo "Hello world, how are you?"
                 '''
            } 
        }
        stage("clean workspace"){
            steps {
                cleanWs()
            }
        }
    }
    
}