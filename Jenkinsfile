pipeline{
  agent { label 'Slave1' }
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
