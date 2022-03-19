pipeline{
    agent{
        label "master"
    }
    options([
  parameters([
    choice(name: 'choices', choices: ['a','b','c'], description: '3 choices')
    
  ])
])
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
