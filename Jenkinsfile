pipeline{
    agent any

    stages{
        stage ('Compile Stage') {
            steps{
                withMaven(maven : '') {
                    sh 'mvn clean'
                }
            }

        }

        stage ('Testing Stage') {
            steps{
                withMaven(maven : '') {
                    sh 'mvn test'
                }
            }
        }

        stage ('Deployment Stage') {
            steps{
                withMaven(maven : '') {
                    sh 'mvn deploy'
                }
            }

        }
    }
        
}