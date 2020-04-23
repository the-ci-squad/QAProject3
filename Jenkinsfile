  
pipeline{
        agent any
        stages{
            stage('test petclinic services'){
                steps{
                      sh """
                      ssh -i ~/id_rsa app-dev@51.145.17.150 <<EOF
                      ls -al
                    
                   
                       """
                }
             }
             stage('launch petclinic'){
                steps{
                      sh """                  
                      ssh -i ~/id_rsa app-dev@51.145.17.150 <<EOF
                      ls -al
                      rm -rf QAProject3
                      git clone --single-branch --branch stef-develop https://github.com/the-ci-squad/QAProject3
                      cd QAProject3/petclinic/spring-petclinic-backend/spring-petclinic-rest/
                      docker start rest || docker run --name rest -p 9966:9966 springcommunity/spring-petclinic-rest
          
                      """
               }
            }
        }    
}
