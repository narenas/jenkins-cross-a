pipeline { 
    agent any 

    triggers {
        eventTrigger simpleMatch("SimpleTrigger")
    }

    stages {
        stage ('Deploy') {
            steps {
                echo 'Deploying in prod'
                sh "./deploy.sh"
            }
        }
    }

}