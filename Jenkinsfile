
pipeline {
  agent any

  stages {
    
    stage('Enforcing Formatting') {
      steps {
        script {
            sh 'echo "formatting good\n"'
            sh 'env'
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
