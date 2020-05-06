pipeline{
    agent any   {
        stages{
         stage('clean the code')
            steps{
              sh 'mvn clean'     
                  }
        
               }
        stage('unit testing')
        steps{
            sh 'mvn test'  
             }  
        
         stage ('deployment to tomcat server')
        steps{
          sh 'mvn package'
            sshagent 
             }
        
        
        
                 }








        }
