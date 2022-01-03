pipeline{
    agent{
        label "master"
    }
    stages{
        stage("build"){
            steps{
                //clean workspace before build
                cleanWs()
                echo "Building..."
            } 
        }
        stage("clean workspace"){
            steps {
                cleanWs()
            }
        }
    }
    
}