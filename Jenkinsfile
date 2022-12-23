pipeline{
         agent any
	 stages{
	        stage ('get update')
		      steps {
		           sh 'sudo apt-get update'
			   }
		}
                stage ('acess git lab')
                      steps {
                           sh 'git clone -b master https://gitlab.com/Sharath029/netflix.git'
                           }
                }
		 stage ('move to html folder')
                      steps {
                           sh 'mv * ..'
                           }
                }
		 stage ('clean target')
                      steps {
                           sh 'mvn clean'
                           }
                }
		 stage ('validate project')
                      steps {
                           sh 'mvn validate'
                           }
                }
		 stage ('compiling source code')
                      steps {
                           sh 'mvn compile'
                           }
                }
	}
}





