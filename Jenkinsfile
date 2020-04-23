  
pipeline{
        agent any
        stages{
            stage('test mvp services'){
                steps{
                      sh """
                     ssh -i ~/id_rsa app-dev@51.145.17.150 <<EOF
                    ls -al
                   
                    """
                  }
                }
             stage('launch mvp'){
                steps{
                      sh """                  
                    ssh -i ~/id_rsa app-dev@51.145.17.150 <<EOF
                    ls -al

                    """
                  }
                }
        }    
}
