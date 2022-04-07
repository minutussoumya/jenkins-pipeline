pipeline{
    agent {label 'ubuntu'}
    stages {
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Testing') {
            steps {
                echo 'Testing'
            }           
        }
        stage("Deploying") {
            steps {
                echo 'Deploying'
            }
        }
        
    }
    post 
    {
        always
        {
            emailext body: 'summary of the pipeline status', subject: 'pipeline status', to: 'kamatesoumya111@gmail.com'
            
        }
    }
}
