pipeline {
  agent any
  stages {
    stage('copiando carpeta de trabajo') {
      steps {
        sh '#!/bin/bash'
        sh 'carpeta="/var/jenkins_home/workspace/tarea2/pagina_web"'
	sh 'if [ -d $carpeta ]; then rm -rfd $carpeta fi'
	sh 'git clone https://github.com/Nokia2k/pagina_web.git'
      }
    }
    stage('colocando en volumen la carpeta') {
      steps {
        sh 'cp $carpeta/index.html /var/www/index.html'
      }
    }

  }
}
