pipeline{
    agent any
    stages{
        stage("Initial Code"){
            steps{
                sh """ echo "Running Pipline Script" """
            }
        }
        stage("Deployment"){
            when{
                branch 'web-service'
            }
            steps {
                sh """
                echo "Building Artifact"
                """

                sh """
                echo "Deploying Code"
                """
            }
        }
    }

}
