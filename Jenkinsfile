pipeline{
  agent {
        docker { 
            image 'python:fattah'
            //-v /docker/volumes/pythonfattah:/srv
            //--mount source=/docker/volumes/pythonfattah,target=/python/results
            args '--name jenkinsbuildenv -v /docker/python/pythonfattah'
            
        }
    }
  stages {
    stage ("echo") {
      steps {
        sh 'echo "salam - $(date)" >> /python/results/firstpipeline.txt '
      }
    }
  }
}
