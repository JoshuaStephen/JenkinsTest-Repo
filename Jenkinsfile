pipeline{
    agent any
    stages{
        stage("Initial Code"){
            steps{
                sh """ echo "Running Pipline Script" """
            }
        }
        stage("Deployment"){
//             when{
//                 branch 'front-end'
//             }
            steps {
                sh """
                echo "Building Artifact - Front End"
                """

                sh """
                echo "Deploying Code - Front End"
                """
            }
        }
    }

}
