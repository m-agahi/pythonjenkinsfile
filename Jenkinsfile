pipeline{
  agent {
        docker { 
            image 'python:fattah'
            args '--rm --name jenkinsbuildenv --mount source=/docker/volumes/pythonfattah,target=/python/results'         
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
