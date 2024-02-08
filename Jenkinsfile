pipeline {
  agent any
  stages {
    stage('comprobando index.html') {
      steps {
        sh '''#!/bin/bash
        indice=/var/www/index.html
	ws=/var/jenkins_home/workspace/Tarea3
	if [ -e $indice ]; then rm -rf $indice; fi'''
      }
    }
    stage('colocando en volumen el archivo') {
      steps {
        sh 'cp $ws/index.html $indice'
      }
    }

  }
}
