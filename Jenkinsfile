pipeline {
  agent any
  stages {
    stage('Clean Reports')
    {
      steps{
        echo '********* Cleaning Workspace Stage Started **********'
        
        echo '********* Cleaning Workspace Stage Finished **********'
      }
    }
    
    stage('Build Stage') {
      steps {
        echo '********* Build Stage Started **********'
       
        echo '********* Build Stage Finished **********'
        }
    }
    stage('Testing Stage') {
      steps {
        echo '********* Test Stage Started **********'
        
        echo '********* Test Stage Finished **********'
      }   
    }
    stage('Configure Artifactory'){
      steps{
        script {
          
          echo '********* Configure Artifactory Started **********'
             
          echo '********* Configure Artifactory Finished **********'
        }
       }
    }
    stage('Sanity check') {
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
  post {
        always {
            echo 'We came to an end!'
            
            {
              echo '********* Uploading to Artifactory is Started **********'
             
              echo '********* Uploading Finished **********'
            }
         }

         }
        success {
          echo 'Build Successfull!!'
    }
        failure {
        echo 'Sorry mate! build is Failed :('
    }
        unstable {
            echo 'Run was marked as unstable'
        }
        changed {
            echo 'Hey look at this, Pipeline state is changed.'
        }
    
}
