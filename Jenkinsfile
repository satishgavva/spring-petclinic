pipeline{

agent { label 'mvnode'}
  
  stages{
  
    stage ('clone'){
      
      agent { label 'mvnode'}
      
      steps {
    
    git url:'https://github.com/satishgavva/spring-petclinic.git' , branch : 'springboot3'
        
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
