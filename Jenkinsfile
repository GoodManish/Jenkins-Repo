pipeline{
    agent any

    stages{
        stage ('Compile Stage') {

            steps{
                withMaven(maven : 'MAVEN_3_6_2'){
                    bat 'mvn clean compile'
                }
            }
        }
        stage ('Test Stage') {

            steps{
                withMaven(maven : 'MAVEN_3_6_2'){
                    bat 'mvn clean test'
                }
            }
        }

        stage ('Verify Stage') {

            steps{
                withMaven(maven : 'MAVEN_3_6_2'){
                    bat 'mvn clean verify'
                }
            }
        }



    }

}