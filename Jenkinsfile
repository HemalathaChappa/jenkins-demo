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
                   bat 'start "" /B cmd /c "npx serve -s dist -l 3000" ' 

 
               }
            }
         }
      }  
            
 
