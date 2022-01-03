pipeline{
    agent{
        label "master"
    }
    stages{
        stage("execute some stuff"){
            steps{
                //clean workspace before build
                cleanWs()
                echo "========executing A========"
            } 
        }
        stage("clean workspace"){
            steps {
                cleanWs()
            }
        }
    }
    
}