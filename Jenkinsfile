pipeline{
    agent any

    stages{
        stage ('Compile Stage') {
            steps{
                withMaven(maven : 'maven_3_5_0') {
                    sh 'maven clean'
                }
            }

        }

        stage ('Testing Stage') {
            steps{
                withMaven(maven : 'maven_3_5_0') {
                    sh 'maven test'
                }
            }
        }

        stage ('Deployment Stage') {
            steps{
                withMaven(maven : 'maven_3_5_0') {
                    sh 'maven deploy'
                }
            }

        }
    }
        
}