pipeline {    
	
	//build environment
	agent any 
    
	//build stages
	stages {
	
        stage('Git Download') {		
            steps {
				
                git credentialsId: 'Git-token', url: 'https://github.com/dilippce88/DoodleProjects.git'
				
				echo " Git Downlaoded Sucessfully"
            }
        }
		
		stage('Run cmd') {		
            steps {
			
                echo 'Running Cmd!' 
				
				bat'''echo "Fix this"'''			
				
				
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
