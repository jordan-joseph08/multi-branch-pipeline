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
                 echo "Hello"
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