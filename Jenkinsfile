pipeline{

agent any 
  
  stages{
  
    stage ('clone'){
      
      steps {
    
    git url :'https://github.com/satishgavva/spring-petclinic.git' , branch 'hacking/mysql'
        
      }
    
    }
    
    stage('build'){
    
      steps {
      
      sh 'mvn package'
      
      }
    
    
    }
    
    
  
  
  
  }





}
