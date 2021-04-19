pipeline {
      agent  none
      stages {
          stage('gitscm'){
                agent {
                    label 'mljen'
                } 
               steps {
                     echo "hello git"
                     sh 'sleep 50'
              }
        }
         stage('build'){
                agent {
                   label 'mljen'
              } 
               steps {
                      echo "hello git"
                      sh 'sleep 50'
             }
        }
    }
}
