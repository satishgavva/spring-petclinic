pipeline{

agent { label 'mnode'}
  
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