pipeline {
    agent any

    stages {
    
         stage('Install Dependencies') {

              steps {
                  bat 'npm install'
              }
          }          

          stage('Build React App') {
              steps {
                  bat 'npm run build'
              }   

           }
           
           stage('Deploy React App') {
               steps {
                   bat 'set JENKINS_NODE_COOKIE=dontKillMe && start "" /B npx serve -s dist -l 3000' 

 
               }
            }
         }
      }  
            
 
