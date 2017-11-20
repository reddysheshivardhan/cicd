pipeline{
		agent any
	  triggers
	{
		pollSCM('* * * * *')
	}
		
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
					  input message: 'Waiting for approval'

				}	
				}
					post
					{
						success
						{
							build 'testjob'

						}
						failure
						{
							echo 'failed'
						}
					}
				}
				
			
				
			}
		
}
