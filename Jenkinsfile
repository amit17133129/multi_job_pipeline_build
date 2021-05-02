pipeline {
      agent  none
      stages {
          stage('Building_Heart_Prection_Pod'){
                steps {
             
                    sh 'sudo kubectl create deployment mlopsheartpred  --image=docker123kubernetes123/heartprediction_mlops:v1   --kubeconfig admin.conf'
                    sh 'sudo kubectl expose deployment mlopsheartpred --type=NodePort  --port=4444   --kubeconfig admin.conf'
                    sh 'sudo kubectl get pods -o wide | grep mlopsheartpred    --kubeconfig admin.conf'
                    
                }
        }
         stage('logs'){
               steps {
                      sh 'sudo kubectl get pods -o wide  --kubeconfig admin.conf'
                      sh 'sudo kubectl get svc    --kubeconfig admin.conf'
             }
        }
    }
}
