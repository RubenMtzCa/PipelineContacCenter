pipeline
{
    agent any
    tools {
        nodejs "node"
    }
    stages{
        stage ('Cloning Git')
        {
            steps {
                git 'https://github.com/RubenMtzCa/PipelineContacCenter.git';
            }
        }
        stage('Install dependencies') 
        {
          steps {
          sh 'npm install'
          sh 'npm install purecloud-flow-scripting-api-sdk-javascript'
                }
        }
        stage ('Test')
        {
            steps{
                sh 'node -v'
            }
        }
    }
}

