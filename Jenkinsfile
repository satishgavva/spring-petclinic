pipeline{

agent {label 'mnode'}

stages {

stage ('scm clone'){

  agent {label 'mnode'}

steps {

git url:'https://github.com/satishgavva/spring-petclinic.git', branch : 'main'
}


}

stage {

agent {label 'mnode'}

steps {

sh 'mvn package'

}


}







}












}