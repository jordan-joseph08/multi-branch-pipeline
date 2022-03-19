pipeline{
    agent{
        label "master"
    }
    
  
    stages{
        stage("clone repo"){
            steps{
                //clean workspace before build
                cleanWs()
                echo "$JOB_NAME"
            } 
        }
        stage('parameters') {
        when {
        expression { env.JOB_NAME == "test-projects-3/test-pipleine/candidate-2" }
        }
        steps {
            parameters {
    choice(name: 'choices', choices: ['a','b','c'], description: '2 choices')
    }
        }
    }
        stage("clean workspace"){
            steps {
                cleanWs()
            }
        }
    }
    
}
