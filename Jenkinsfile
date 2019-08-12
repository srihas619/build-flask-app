
pipeline {
  agent any

  stages {
    
    stage('Build will run on all branches EXCEPT master. Build will finish here otherwise') {
      steps{
	      when {
          expression { env.BRANCH_NAME != 'master' } // if branch is master, build ends here, otherwise continue with the stages below
      	}	
      }
    }

    stage('Enforcing Formatting') {
      steps {
        script {
          ansiColor('xterm') {
            sh "formatting good\n"
            echo "$payload"

          }
        }
      }
    }
      
    stage("Testing make plan") {
      steps {
        script {
            sh "\n====building===="
        }
      }
    }
  }
}
