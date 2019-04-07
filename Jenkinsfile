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
            echo 'Hello Jenkins:Testing1235!'

        }
   
        }
        stage('Build') {
            steps {
            echo 'Hello Jenkins:Testing1234!'

        }
        }
        stage('Test') {
            steps {
            echo 'Hello Jenkins:testing!'

        }
        }
		stage('Deploy'){
		     steps {
            echo 'Hello Jenkins!'

        }
		}

		stage('run-parallel-branches') {
 				steps {
  			parallel(
   					a: {
    		echo "Tests on Linux"
    		sleep 10
   				},
   				b: {	
    	echo "Tests on Windows"
    	sleep 10
  			 }
  			)
		 }
		}

    }

}
