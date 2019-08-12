
pipeline {
  agent any

  stages {
    
    stage('Enforcing Formatting') {
      steps {
        script {
            sh "formatting good\n"
            echo "$payload"
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
