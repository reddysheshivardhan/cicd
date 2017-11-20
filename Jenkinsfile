pipeline{
		
	  triggers
	{
		pollSCM('* * * * *')
	}
		
			stages
			{
				agent any
				stage('bulit')
				{
				    steps{
					    sh 'mvn package'
					      				    
					}
				    post
					    {
						    success
						    {
						    echo 'post 123'
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
