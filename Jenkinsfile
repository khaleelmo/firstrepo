pipeline{

    agent {
        
        node {
        	 label 'master'
             customWorkspace 'C:/Users/mokhalee/Jenkins/workspace'
        }

    }

    
    options {
        timestamps()
        

    }

    stages{
        stage('Checkout') {
        steps {
            echo 'Hello Jenkins! from newbranch1234'

        }
   
        }
        stage('Build') {
            steps {
            echo 'Hello Jenkins! from newbranch'

        }
        }
        stage('Test') {
            steps {
            echo 'Hello Jenkins! from newbranch'

        }
        }
		stage('Deploy'){
		     steps {
            echo 'Hello Jenkins! from newbranch'

        }
		}

		stage('run-parallel-branches') {
 				steps {
  			parallel(
   					a: {
    		echo "Tests on Linux from newbranch"
    		sleep 10
   				},
   				b: {	
    	echo "Tests on Windows from newbranch"
    	sleep 10
  			 }
  			)
		 }
		}

    }

}



