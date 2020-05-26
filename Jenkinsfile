pipeline { 
    agent any 

    triggers {
        eventTrigger simpleMatch("SimpleTrigger")
    }

    stages {
        stage ('Deploy') {
            steps {
                echo 'Deploying in prod'
                sh "chmod 755 deploy.sh && ./deploy.sh"
            }
        }
    }

}