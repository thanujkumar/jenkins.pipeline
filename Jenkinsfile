pipeline {
    //agent { docker { image 'maven:3.3.3' } }
    agent any
    stages {
        stage('build') {
            withMaven(
               maven: 'maven_3.5.4', mavenLocalRepo: '/maven/repo') {
                sh 'mvn --version'
            }
        }
    }
}
