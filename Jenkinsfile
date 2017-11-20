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
