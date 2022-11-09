pipeline{
    agent any
       stages {
           stage("list env var"){
             steps {
               sh "printenv | sort"
             }
           }
           
           stage("using env var"){
             steps {
                 echo "BUILD_NUMBER= ${env.BUILD_NUMBER}"
             }
            } 
            
            stage("extract branch name"){
                steps {
                    echo "BRANCH_NAME= ${env.BRANCH_NAME}"
                        }
            }
        }
}
    
          
