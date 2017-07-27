node {
    checkout scm
    stage('Build and Deploy') {
        withMaven(
            jdk: 'JDK8', 
            maven: 'M3', 
            mavenSettingsConfig: 'MavenReadOnly') {
            sh "mvn clean install"
        }
    }
}
