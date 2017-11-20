pipeline{
		agent any
		
			stages
			{
				stage('bulit')
				{
				    steps{
					    sh 'mvn package'
					      				    
					}
				    post
					    {
						    success
						    {
						    echo 'post'
					            archiveArtifacts '**/target123/*.war'
						    }
					    }	
				 	
				}
				
			
				
			}
		
}
