pipeline {    
	
	//build environment
	agent any 
    
	//build stages
	stages {
	
        stage('Stage 1') {		
            steps {
                echo 'Hello Stage1!' 
            }
        }
		
		stage('Stage 2') {		
            steps {
                echo 'Hello STage2!'
                
            }
        }
        
    }
	
	//post action
	post {
	
		always{
		
		echo "Something Something"
		
		}		
		
		success{
		
		echo "success POST"
		
		}
		
		failure{
		
		echo "Fail"		
		
		}
		
		aborted{		
		
		echo "Aborted"		
		
		}
			
	
	}	
	
}
