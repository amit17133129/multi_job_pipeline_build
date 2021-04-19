  
pipeline {
      agent  none
      stages {
          stage('gitscm'){
                agent {
                    label 'mljen'
                } 
               steps {
                     echo "hello git  1111"
                     sh 'sleep 50'
              }
        }
         stage('build'){
                agent {
                   label 'mljen'
              } 
               steps {
                      echo "hello git 111111"
                      sh 'sleep 50'
             }
        }
    }
}
