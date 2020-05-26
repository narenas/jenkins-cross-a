pipeline { 
    agent any 

    triggers {
        eventTrigger simplematch("SimpleTrigger")
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