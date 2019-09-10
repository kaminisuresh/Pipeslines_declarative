pipeline {
    agent none
  tools {
    
   maven 'Maven-3' 
  }
	
    stages {
        stage("build and deploy on Slave1 and Slave2") {
            parallel {
                stage("Slave1") {
                    agent {
                        label "Slave1"
                    }
                    stages {
                        stage("build") {
                            steps {
                                sh "mvn clean install"
                            }
                        }
                        
                    }
                }

                stage("linux") {
                    agent {
                        label "Slave2"
                    }
                    stages {
                        stage("build") {
                            steps {
                                sh "mvn clean isntall"
                            }
                        }
                        
                    }
                }
            }
        }
    }
}
