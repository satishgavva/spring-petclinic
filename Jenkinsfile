pipeline{

agent any 
  
  stages{
  
    stage ('clone'){
      
      steps {
    
    git url :'https://github.com/satishgavva/spring-petclinic.git' , branch 'efficient-webjars'
        
      }
    
    }
    
    stage('build'){
    
      steps {
      
      sh 'mvn package'
      
      }
    
    
    }
    
    
  
  
  
  }





}
