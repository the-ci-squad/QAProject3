//jenins for angualr
//clone angular repo
//cd into repo
//run built-in tests ng test, e2e
//run backend (rest server)
//deploy actual frontend 
pipeline{
	agent any
	//tools { 
        //	maven 'Maven 3.3.9' 
        //	jdk 'jdk8' 
    	//}
	stages{
	    stage('Deploy'){
		steps{
		    sh '''
		    pwd
		    ssh -i ~/id_rsa app-dev@51.145.17.150 << EOF
		    rm -rf spring-petclinic-rest
		    rm -rf spring-petclinic-angular
		    git clone --single-branch --branch stef-develop https://github.com/the-ci-squad/QAProject3/tree/stef-develop/petclinic/spring-petclinic-backend/spring-petclinic-rest
		   
		    git clone --single-branch --branch stef-develop https://github.com/the-ci-squad/QAProject3/tree/stef-develop/petclinic/spring-petclinic-front/spring-petclinic-angular
		    cd spring-petclinic-rest 
		    docker start rest || docker run --name rest -p 9966:9966 springcommunity/spring-petclinic-rest

		    cd .. 
		    cd spring-petclinic-angular



		    '''
		}
	    }
	}
}
