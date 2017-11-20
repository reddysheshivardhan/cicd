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
					            archiveArtifacts '**/target/*.war'
						    }
					    }	
				 	
				}
				stage('deploy')
				{
					steps{
				  timeout(time: 5, unit: 'HOURS') {
					    // some block
					  echo 'Time out'
				}	
				}
				}
				
			
				
			}
		
}
