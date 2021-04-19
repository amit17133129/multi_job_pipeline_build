pipeline {
      agent  none
      stages {
          stage('gitscm'){
                agent {
                    label 'myslavw1'
                } 
                steps {
             
                    sh 'sudo kubectl run myos123  --image=docker123kubernetes123/nnnnnnnnnnewwww:v1'
                    sh 'sudo kubectl expose pod myos123 --type=NodePort  --port=4444'
                    sh 'sudo kubectl get pods -o wide | grep myos123'
                    
                }
        }
         stage('build'){
                agent {
                   label 'myslavw1'
              } 
               steps {
                      echo "hello git"
                      sh 'sudo kubectl get pods'
             }
        }
    }
}
