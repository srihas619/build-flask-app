
pipeline {
  agent any

  stages {
    
    stage('Enforcing Formatting') {
      steps {
        script {
            sh 'echo "formatting good\n"'
            sh 'echo "$payload"'
        }
      }
    }
      
    stage("Testing make plan") {
      steps {
        script {
            sh 'echo "\n====building===="'
        }
      }
    }
  }
}
