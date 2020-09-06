pipleline {
    agent any

    stages {
        
        stage ('Initialization') {
            steps {
                sh 'echo "Starting the CI Pipeline"'
            }
        }

        stage ('Build') {
            steps {
                sh '''
                    export MYSQL_USER=root
                    export MYSQL_DATABASE=dvna
                    export MYSQL_PASSWORD=Passw0rd
                    export MYSQL_HOST=127.0.0.1
                    export MYSQL_PORT=3306
                    npm install
                    '''
            }
        }   
    }
}
