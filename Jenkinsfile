pipeline {
    agent any
    tools { 
        maven 'maven' // Tool name from Jenkins "Global Tool Configuration"
        jdk 'java8' // Tool name from Jenkins "Global Tool Configuration"
    }	
    stages {
        stage ('Clone') {
            steps {
                git branch: 'master', url: "https://github.com/abhijeetparia/Simple-Java-Maven.git"
            }
        }
        stage('Build') { 
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
