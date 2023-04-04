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
                branch 'front-end'
            }
            steps {
                sh """
                echo "Building Artifact"
                """

                sh """
                echo "Deploying Code"
                """
            }
            when{
                branch 'main'
            }
            steps {
                sh """
                echo "Building Artifact on Main branch"
                """
            }
        }
    }

}