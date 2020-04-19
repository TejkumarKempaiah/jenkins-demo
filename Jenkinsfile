pipeline {
    agent any 
    stages {
        stage('Clone') {
            steps {
                echo "checking out the repo"
                git 'https://github.com/edureka-devops/jenkins-demo.git'
            
            }
        }
        stage('build'){
            steps {
                echo "building the project"
                sh "cd MavenProject ; mvn clean install ; pwd"
            }
        }
        
        stage('Archieve Artifacts'){
            steps {
                echo "archiving the artifacts"
               
            }
            
        }
        stage('Deployment') {
          
            steps {
                script {
                    echo "deployment"
                   
                }
            }
        }
        stage('publish html report') {
            steps{
                echo "publishing the html report"
                
            }
        }
        stage('clean up') {
            steps {
                echo "cleaning up the workspace"
         
            }
        }
        stage("Metrics"){
            steps{
            echo "Metrix generation"
         
            }
        
    }
}
        
