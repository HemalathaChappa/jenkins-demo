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
                   bat 'start "" /B cmd /c "npm run preview -- --host 0.0.0.0 --port 3000" ' 

 
               }
            }
         }
      }  
            
 
