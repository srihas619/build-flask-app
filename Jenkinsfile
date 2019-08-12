
pipeline {
  agent any

  stages {
    stage('Build will run on all branches EXCEPT master. Build will finish here otherwise') {
      when {
          expression { env.BRANCH_NAME != 'master' } // if branch is master, build ends here, otherwise continue with the stages below
      }

    stages {
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
  post {
    // not sure if wanted
    always {
      deleteDir()
    }
  }
}
// vim: autoindent expandtab shiftwidth=2
