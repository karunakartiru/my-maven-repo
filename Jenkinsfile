pipeline {
    agent any

   stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/karunakartiru/my-maven-repo.git'

                // Run Maven on a Unix agent.
                sh "/opt/apache-maven-3.8.8/bin/mvn clean deploy"

                // To run Maven on a Windows agent, use
                // bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }

           }/
    }
}
