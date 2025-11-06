pipeline {
    agent any
    parameters {
        choice(name: 'Env', choices: ['dev', 'test', 'prod'], description: 'select one env here:')
    }
    stages {
        stage('select') {
            steps {
                script {
                    if (params.Env == 'dev') {
                        echo "Running for DEV environment"
                    } else if (params.Env == 'test') {
                        echo "Running for TEST environment"
                    } else {
                        echo "Running for PROD environment"
                    }
                }
            }
        }
    }
}
