pipeline {
  agent any
  stages {
    stage('Printing') {
      parallel {
        stage('Printing') {
          steps {
            echo 'Hello MyWorld'
          }
        }
        stage('Printe Another') {
          steps {
            echo 'Hello another world!'
          }
        }
      }
    }
    stage('Fehler Signal') {
      steps {
        error 'Ich bin ein Fehler Signal'
      }
    }
    stage('Ich schlafe') {
      steps {
        sleep 10
      }
    }
    stage('File writing') {
      steps {
        writeFile(file: 'Testfile', text: 'Hallo, ich bin ein Testfile')
      }
    }
  }
}