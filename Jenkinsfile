pipeline {
    //agent { docker { image 'maven:3.3.3' } }
    agent any
    stages {
        stage('build') {
            steps {
             withMaven(
                 maven: 'maven_3.5.4', mavenLocalRepo: '/m2_repo') {
                sh 'mvn clean compile'
              }
            }
        }
    }
}
