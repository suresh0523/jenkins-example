pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                //withMaven(maven : 'maven_3_5_0') {
                    sh '/opt/maven/bin/mvn clean compile'
               // }
            }
        }

        stage ('Testing Stage') {

            steps {
                //withMaven(maven : 'maven_3_5_0') {
                    sh '/opt/maven/bin/mvn test'
                //}
            }
        }


        stage ('Deployment Stage') {
            steps {
                //withMaven(maven : 'maven_3_5_0') {
                    sh '/opt/maven/bin/mvn deploy'
                //}
            }
        }
    }
}
