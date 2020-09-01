pipeline{
  agent {
        docker { 
            image 'python:fattah'
            //--mount source=/docker/volumes/pythonfattah,target=/python/results
            args '--rm --name jenkinsbuildenv -v /docker/volumes/pythonfattah:/python/results:rw'
        }
    }
  stages {
    stage ("echo") {
      steps {
        sh 'echo "salam - $(date) >> /python/results/firstpipeline.txt '
      }
    }
  }
}
