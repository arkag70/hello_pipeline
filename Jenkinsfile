pipeline {
    agent {docker {image 'node:18.16.0-alpine'} }

    stages {
  	    stage('build') {
      steps {
      	cd 'build' || mkdir 'build' && cd 'build'
        cmake ../ && make
        cd ../
      }
    }
  }
}