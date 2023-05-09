pipeline {
    agent any
    tools{
        maven 'M2_HOME'
    }    
    Stages('build') {
          sleps {
             sh 'mvn clean'
             sh 'mvn install'
             sh 'mvn packages'
       }
    }
    stage('test'){
       steps {
         echo "Test Step "
       }
    }
    stage('Deploy'){
       steps {
         echo "Deploy Step"
       }
    }
    stage('Docker'){
       steps {
         echo "Image step"
       }
    }
  } 
