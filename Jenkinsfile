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
                echo "Testing..."
                echo "Deployment..."
            } 
        }
        stage("clean workspace"){
            steps {
                cleanWs()
            }
        }
    }
    
}