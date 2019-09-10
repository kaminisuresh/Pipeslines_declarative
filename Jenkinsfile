pipeline{
  agent { label 'Slave2' }
  tools { 
    
   maven 'Maven-3'
    jdk 'JDK-8'
  }
stages{

stage('build'){
steps{
sh 'mvn clean package'
}

}


}

}
