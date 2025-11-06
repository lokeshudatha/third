pipeline{
    agent any
    parameters{
        choice(name: 'Env', choices: ['dev', 'test', 'prod'], description: 'select one env here: ')
    }
    stages{
        stage('select'){
            when{
                expression{
                    return params.Env == 'dev'
                }
            }
            steps{
                script{
                    if(params.Env == 'test'){
                        echo "condition is satify"
                    } else{
                        error("its error block")
                    }
                }
            }
        }
    }
}
