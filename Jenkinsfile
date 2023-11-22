pipeline {
  agent any
  stages {
    stage('github')
    {
      steps{
        echo '********* Cleaning Workspace Stage Started **********'
        
        echo '********* Cleaning Workspace Stage Finished **********'
      }
    }
    
    stage('mvn Build Stage') {
      steps {
        echo '********* Build Stage Started **********'
       
        echo '********* Build Stage Finished **********'
        }
    }
    stage('docker image build Stage') {
      steps {
        echo '********* Test Stage Started **********'
        
        echo '********* Test Stage Finished **********'
      }   
    }
    stage('helm stage'){
      steps{
        script {
          
          echo '********* Configure Artifactory Started **********'
             
          echo '********* Configure Artifactory Finished **********'
        }
       }
    }
    stage('kubernetes') {
            steps {
               echo '*******************sanity check*************************'
            }
     }
stage('Deployment Stage'){
            steps{
               
                echo '********* Deploy Stage Started **********'
               
                echo '********* Deploy Stage Finished **********'
            }
    }
  } 
}
