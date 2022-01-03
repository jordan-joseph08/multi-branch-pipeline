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
                 echo "Hello world, how are you doing. Jordan here"
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