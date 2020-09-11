pipeline{
  agent {
        docker {
            label 'docker1'
            image 'python:fattah'
            //-v /docker/volumes/pythonfattah:/srv
            //--mount source=/docker/volumes/pythonfattah,target=/python/results
            args '--name jenkinsbuildenv -v /docker/volumes/pythonfattah:/python/results'
            
        }
    }
  stages {
    stage ("echo") {
      steps {
        sh 'echo "salam - $(date)"'
        sh 'sleep 200'
      }
    }
  }
}
