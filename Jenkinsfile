pipeline{

agent any 
  
  stages{
  
    stage ('clone'){
      
      steps {
    
    git url :'https://github.com/satishgavva/spring-petclinic.git' , branch 'main'
        
      }
    
    }
    
    stage('build'){
    
      steps {
      
      sh 'mvn package'
      
      }
    
    
    }
    
    
  
  
  
  }





}
