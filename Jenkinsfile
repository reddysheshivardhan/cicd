pipeline{
		agent any
		
			stages
			{
				stage('bulit')
				{
				    steps{
					    sh 'mvn package'
					    post
					    {
						    echo 'post'
					    }
					    echo 'step 2'
					    echo 'step3'
					    
					}
				 	
				}
				stage('arch')
				{
					steps
					{
					echo 'archive'
						archiveArtifacts '**/target/*.war'
					
					}
				}
			
				
			}
		
}
