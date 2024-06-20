pipeline {
  agent any
  stages {
    stage('Design Preparation') {
      steps {
        echo 'Design'
      }
    }

    stage('Design Build') {
      steps {
        echo 'Build'
      }
    }

    stage('Design Review Request') {
      steps {
        echo 'Design Review Request'
      }
    }

    stage('MIL') {
      parallel {
        stage('MIL Preparation') {
          steps {
            echo 'MIL Preparation'
          }
        }

        stage('Impl Preparation') {
          steps {
            echo 'Impl Preparation'
          }
        }

      }
    }

  }
}