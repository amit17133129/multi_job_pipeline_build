pipeline {
      agent any
      stages {
          stage('BuildingHeartPrectionPod'){
                steps {
                    sh 'sudo kubectl create deployment mlopsheartpred  --image=docker123kubernetes123/heartprediction_mlops:v1   --kubeconfig /root/admin.conf'
                    sh 'sudo kubectl expose deployment mlopsheartpred --type=NodePort  --port=4444   --kubeconfig /root/admin.conf'
                    sh 'sudo kubectl get pod -o wide | grep mlopsheartpred    --kubeconfig /root/admin.conf'
                    
                }
        }
         stage('logs'){ 
               steps {
                      sh 'sudo kubectl get pod -o wide  --kubeconfig /root/admin.conf'
                      sh 'sudo kubectl get svc    --kubeconfig /root/admin.conf'
             }
        }
    }
}
