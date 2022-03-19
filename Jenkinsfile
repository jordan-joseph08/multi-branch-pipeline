pipeline{
    agent{
        label "master"
    }
    
   if (env.JOB_NAME == 'test-projects-3/test-pipleine/candidate-2') 
                        {
                        parameters {
choice(name: 'choices', choices: ['a', 'b'], description: '2 choices')
}
                            
                       }
    
    else {
       parameters {
choice(name: 'choices', choices: ['a', 'b', 'c'], description: '3 choices') 
    }
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
