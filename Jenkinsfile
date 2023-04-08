pipeline {
    agent any
    
    tools
    {
       maven "Maven"
    }

    stages {
        stage('clone') {
            steps {
                git credentialsId: 'github', url: 'https://github.com/sandeepbselemane/sample_java_maven_project.git'
            
                sh 'ls' 
            }
        }
        stage('build') {
            steps {
                sh 'mvn package'
            }
        }
        stage('deploy') {
            steps {
                sh '''
                echo $variable1
                '''
                
            }
        }
    }
}
