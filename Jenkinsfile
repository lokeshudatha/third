pipeline{
    agent any
    environment{
        A = "lokesh"
        B = "udatha"
    }
    stages{
        stage('String'){
            when{
                expression{
                    return env.A == "lokesh"
                }
                steps{
                    echo "okay, this is working"
                }
            }
        }
    }
}
