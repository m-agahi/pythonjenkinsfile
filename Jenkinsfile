pipeline{
  agent {
        docker { 
            image 'python:fattah'
            //-v /docker/volumes/pythonfattah:/srv
            //--mount source=/docker/volumes/pythonfattah,target=/python/results
            //args '--rm --name jenkinsbuildenv --mount source=pythonfatah,target=/srv'
            
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
