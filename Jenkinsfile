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
                 echo "Building"
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