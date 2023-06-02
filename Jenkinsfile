pipeline{

  agent { label 'mnode'}
  tools {
        maven 'MAVEN9'
        jdk  'java19' 
    }
  parameters {  

    choice(name: 'main', choices: ['wavefront', 'springboot3', 'hacking/mysql', 'efficient-webjars'], description: 'Pick something')
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
    
    stage('parameter'){

      agent{label 'mnode'}

      steps {

        echo "main: ${params.main}"

      }



    }
    
  
  
  
  }


}
