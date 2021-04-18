pipeline {
      agent  none
      stages {
          stage('gitscm'){
                agent {
                    label 'myk8sslave1'
                } 
               steps {
                     echo "hello git"
                     sh 'sleep 50'
              }
        }
         stage('build'){
                agent {
                   label 'myk8sslave1'
              } 
               steps {
                      echo "hello git"
                      sh 'sleep 50'
             }
        }
    }
}
