node {
    checkout scm
    stage('Build and Deploy') {
        withMaven(
            jdk: 'JDK8', 
            maven: 'M3', 
            mavenSettingsConfig: 'maven-settings-for-supply-chain-build-job') {
            sh "mvn clean deploy"
        }
    }
}