pipeline{
  agent {
        docker { 
            image 'python:fattah'
            args '--volume pythonfattah:/python/results'         
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
