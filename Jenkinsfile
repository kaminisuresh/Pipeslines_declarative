pipeline{
  agent { label 'Slave2' }
  stages{

stage('build'){
steps{
  rtMavenRun (
                    tool: Maven-3, // Tool name from Jenkins configuration
                    goals: 'clean install'
                    
                )

}

}


}

}
