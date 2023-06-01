pipeline{

agent any 
  
  stages{
  
    stage ('clone'){
      
      agent { label 'mvnode'}
      
      steps {
    
    git url:'https://github.com/satishgavva/spring-petclinic.git' ,  branch : 'main'
        
      }
    
    }
    
    stage('build'){
      
      agent { label 'mvnode'}
    
      steps {
      
      sh 'mvn package'
      
      }
    
    
    }
    
    
  
  
  
  }





}
