pipeline{
    agent any
    parameters{
        string(name: 'user', defaultValue: 'lokesh', description: 'Enter your name here: ')
    }
    stages{
        stage('para'){
            when{
                expression{
                    return params.user == 'lokesh'
                }
            }
            steps{
                sh 'mkdir lokesh'
                sh 'cd lokesh'
            }
        }
    }
}
