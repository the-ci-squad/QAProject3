  
pipeline{
        agent any
        stages{
            stage('test petclinic services'){
                steps{
                      sh """
                      ssh -i ~/id_rsa app-dev@51.145.17.150 <<EOF
                      ls 
                    
                   
                       """
                }
             }
             stage('launch petclinic'){
                steps{
                      sh """                  
                      ssh -i ~/id_rsa app-dev@51.145.17.150 <<EOF
        
                      rm -rf QAProject3
                      git clone --single-branch --branch stef-develop https://github.com/the-ci-squad/QAProject3
                      sudo apt install -y kubectl
                      sudo az aks install-cli
                      cd QAProject3/petclinic/kubernetes-petclinic
                      kubectl apply -f api.yml
                     
                      
                      
                      
                      
         
          
                      """
               }
            }
        }    
}
