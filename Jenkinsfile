pipeline {
      agent  none
      stages {
          stage('gitscm'){
                agent {
                    label 'mlopsnode'
                } 
                steps {
             
                    sh 'sudo kubectl create deployment mlops  --image=docker123kubernetes123/updated_keras_mlops:v4'
                    sh 'sudo kubectl expose deployment mlops --type=NodePort  --port=4444'
                    sh 'sudo kubectl get pods -o wide | grep mlops'
                    
                }
        }
         stage('build'){
                agent {
                   label 'mlopsnode'
              } 
               steps {
                      echo "hello git new file"
                      sh 'sudo kubectl get pods -o wide'
             }
        }
    }
}
