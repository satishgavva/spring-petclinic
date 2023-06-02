pipeline{

  agent { label 'mnode'}
  tools {
        maven 'MAVEN9'
        jdk  'java19' 
    }
      
  triggers {
        cron('* * * * *')
    }
  
  stages{
  
    stage ('clone'){
      
      agent { label 'mnode'}
      
      steps {
    
          git url:'https://github.com/satishgavva/spring-petclinic.git' , branch : 'main'
        
      }
    
    }
    
    stage('build'){
      
      agent { label 'mnode'}
    
      steps {
      
      sh 'mvn package'
      
      }
    
    
    }
    
    


    }
    
  
  
  
  }

