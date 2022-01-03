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
                 ls
                 git init
                 git clone https://github.com/tpouche94/multi-branch-pipeline.git
                 ls
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