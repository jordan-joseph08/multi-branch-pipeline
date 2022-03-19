pipeline{
    agent{
        label "master"
    }
    stages('parameters') {
        when {
        expression { env.JOB_NAME == "test-projects-3/test-pipleine/candidate-2" }
        }
        steps {
            parameters {
    choice(name: 'choices', choices: ['a','b','c'], description: '2 choices')
    }
        }
    }
    parameters {
    choice(name: 'choices', choices: ['a','b','c'], description: '3 choices')
    }
    stages{
        stage("clone repo"){
            steps{
                //clean workspace before build
                cleanWs()
                echo "$JOB_NAME"
            } 
        }
        stage("clean workspace"){
            steps {
                cleanWs()
            }
        }
    }
    
}
