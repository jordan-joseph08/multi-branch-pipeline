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
                 echo "$JOB_NAME"
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
